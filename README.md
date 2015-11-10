# Aliyun OSS SDK for Python

## ����
�����ƶ���洢Python SDK��

## ���л���
Python 2.6��2.7��3.3��3.4��3.5

## ��װ����
```bash
$ pip install oss
```

## ����ʹ��
```python
import oss


auth = oss.Auth(access_key_id, access_key_secret)
bucket = oss.Bucket(auth, 'oss-cn-hangzhou.aliyuncs.com', 'my-bucket')

object_name = 'story.txt'

# �ϴ�
bucket.put_object(object_name, 'Ali Baba is a happy youth.')

# ����
bucket.get_object(object_name).read()

# ɾ��
bucket.delete_object(object_name)
```
## ����
����ͨ���������������ò��������AccessKeyID��AccessKeySecret��Endpoint�Լ�Bucket��Ϣ��
```bash
$ export OSS_TEST_ACCESS_KEY_ID=<AccessKeyID>
$ export OSS_TEST_ACCESS_KEY_SECRET=<AccessKeySecret>
$ export OSS_TEST_ENDPOINT=<endpoint>
$ export OSS_TEST_BUCKET=<bucket>
```
Ȼ�����ͨ�����·�ʽ֮һ���в��ԣ�
```bash
$ python -m unitest discover test   # ���Python�汾 >= 2.7
$ nosetests                         # �����װ��nose
$ py.test                           # �����װ��py.test
```
## ����ʹ��

## ע������

## ��ϵ����

## �������
MIT���֤���μ�LICENSE�ļ���