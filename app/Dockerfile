# 使用 Python 3.9 作为基础镜像
FROM python:3.10

# 设置工作目录
WORKDIR /app

# 复制应用程序代码
COPY . /app

# 安装依赖项
RUN pip install --no-cache-dir -r requirements.txt

# 暴露容器端口
EXPOSE 8000

# 运行 FastAPI 应用程序
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]
