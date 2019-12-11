using UnityEngine;

public class GroundManager : MonoBehaviour
{
    // Start is called before the first frame update

    readonly float left = -2.5f, right = 2.5f;
    readonly int init = 6;

    public float SpacingY;

    public float upspeed;

    

    readonly GameObject[] newGround = new GameObject[6];

    void Start()
    {
        for (int i = 0; i < init; i++)
        {

            newGround[i] = Instantiate(Resources.Load<GameObject>("floor"));

            if (i == 0)
            {
                newGround[i].transform.position = new Vector3(0, 0, 0);
            }
            else
            {
                newGround[i].transform.position = new Vector3(newX(), newY(i), 0);
            }
            
        }
    }
    float newY(int l)
    {
        return (- SpacingY * l);
    }
        float newX()
    {
        return Random.Range(left, right);
    }



    int change = 0;
    // Update is called once per frame
    void Update()
    {
        
        
        for (int a = 0; a < init; a++)
        {
            newGround[a].transform.position += new Vector3(0, upspeed, 0);
            if (newGround[a].transform.position.y >= 3.5)
            {
                newGround[a].transform.position = new Vector3(newX(), newGround[a].transform.position.y - SpacingY * init, 0);
            }

        }

        //print(newGround[a].transform.position);
        upspeed += 0.00002f;
    }


    
}
