# MethodOverridingConcept



using System;

namespace MethodOverridingConcept
{
    class BaseClass
    {
        public virtual void Ride()
        {
            Console.WriteLine("this is ride of your Base Man");
        }
    }

    class Derived: BaseClass
    {
        public override void Ride()
        {
            Console.WriteLine("this is ride of your Child Women");
        }

    }
    class Program
    {
        static void Main(string[] args)
        {
            BaseClass baseClassObject = new BaseClass();
            baseClassObject.Ride();

            Derived derived = new Derived();
            derived.Ride();
        }
    }
}
