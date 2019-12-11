using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class player : MonoBehaviour
{
    public float forceX;
    public static bool dead;
    Rigidbody2D Lucky;

    readonly float x1 = -1, x2 = 1, x0 = 0;
    float xmove;

    // Start is called before the first frame update
    void Start()
    {
        dead = false;
        Lucky = GetComponent<Rigidbody2D>();
    }

    // Update is called once per frame
    void Update()
    {
        if (Input.GetKey(KeyCode.LeftArrow))
        {
            xmove = x1;
        }
        else if (Input.GetKey(KeyCode.RightArrow))
        {
            xmove = x2;
        }
        else
        {
            xmove = x0;
        }


        Vector2 playerdirection = new Vector2(xmove, 0);
        Lucky.AddForce(playerdirection * forceX);
     }
}
