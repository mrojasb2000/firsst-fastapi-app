mkdir backend
cd backend

conda init
conda create -n envpy311 python=3.11
conda activate envpy311

pip install fastapi
pip install "uvicorn[standard]"
uvicorn main:app --reload 