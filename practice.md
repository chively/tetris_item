
// 보드에 완성된 행이 있으면 삭제 -> 블럭 전부 삭제?

    void DestroyAllColumn()
    {
        bool isCleared = false;

        foreach (Transform column in boardNode)
        {
            if (column.childCount >= 1)
            {
                foreach (Transform tile in column)
                {
                    Destroy(tile.gameObject);
                }
                column.DetachChildren();
                isCleared = true;
            }
            
        }
        
    }

// 특정 라인 삭제

    void DestroySpecificColumn()
    {
        bool isCleared = false;
        
        foreach (Transform column in boardNode)
        {
            if (특정라인 찾아야함)
            {
                foreach (Transform tile in column)
                {
                    Destroy(tile.gameObject);
                }
                column.DetachChildren();
                isCleared = true;
            }
            
        }
        
    }


// 속도 빠르게 하기?

    void SpeedUp()
    {
        fallCycle = fallCycle - 0.1f;
    }

// 일정 시간 동안 빠른 속도 유지

    void SpeedUp10sc
    {
        제어문
            fallCycle = 0.5f;
    }



