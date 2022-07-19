# Eungram
22/07/19
 장고 실행
 오류 : templates가 없다고 뜸.
 해결 : settings.py에 
import os
BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
TEMPLATE_DIR = os.path.join(BASE_DIR, 'templates') 
코드 추가하고 Templates 내에 있는 'DIRS'에 TEMPLATE_DIR 작성
