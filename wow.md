import { Card, CardContent } from "@/components/ui/card" import { Button } from "@/components/ui/button" import { Sparkles, Heart, Gift, Cake } from "lucide-react" import { motion } from "framer-motion"

export default function GhepiraBirthdaySite() { return ( <main className="min-h-screen bg-pink-100 flex flex-col items-center justify-center p-6"> <motion.div initial={{ opacity: 0, scale: 0.8 }} animate={{ opacity: 1, scale: 1 }} transition={{ duration: 0.8 }} className="text-center mb-6" > <h1 className="text-4xl font-bold text-pink-600 mb-2">Happy 17th Birthday 🎂</h1> <h2 className="text-2xl text-pink-500">to my sweetest Ghephira Khansa Tadzkia 🍓</h2> </motion.div>

<motion.div 
    initial={{ y: 50, opacity: 0 }} 
    animate={{ y: 0, opacity: 1 }} 
    transition={{ delay: 0.5, duration: 0.6 }}
    className="grid grid-cols-1 sm:grid-cols-2 gap-4 max-w-xl"
  >
    <Card className="bg-white rounded-2xl p-4 shadow-lg border-pink-300 border-2">
      <CardContent className="flex flex-col items-center text-center">
        <Sparkles className="text-pink-400 mb-2" size={36} />
        <p className="text-lg text-pink-600 font-semibold">
          makasih udah lahir ke dunia ini dan jadi orang yang bikin aku senyum tiap hari
        </p>
      </CardContent>
    </Card>

    <Card className="bg-white rounded-2xl p-4 shadow-lg border-pink-300 border-2">
      <CardContent className="flex flex-col items-center text-center">
        <Heart className="text-red-400 mb-2" size={36} />
        <p className="text-lg text-pink-600 font-semibold">
          aku bersyukur banget bisa ketemu kamu, cewek strawberry tersayangku 🍓
        </p>
      </CardContent>
    </Card>

    <Card className="bg-white rounded-2xl p-4 shadow-lg border-pink-300 border-2">
      <CardContent className="flex flex-col items-center text-center">
        <Gift className="text-pink-500 mb-2" size={36} />
        <p className="text-lg text-pink-600 font-semibold">
          semoga tahun ini kamu makin bahagia, sehat selalu dan tetap jadi ghefira yang aku sayang 🧸
        </p>
      </CardContent>
    </Card>

    <Card className="bg-white rounded-2xl p-4 shadow-lg border-pink-300 border-2">
      <CardContent className="flex flex-col items-center text-center">
        <Cake className="text-pink-500 mb-2" size={36} />
        <p className="text-lg text-pink-600 font-semibold">
          semoga kamu dan labubu kamu selalu tersenyum terus, kayak hari ini 💗
        </p>
      </CardContent>
    </Card>
  </motion.div>

  <motion.div 
    initial={{ opacity: 0, y: 20 }}
    animate={{ opacity: 1, y: 0 }}
    transition={{ delay: 1.2, duration: 0.5 }}
    className="mt-8"
  >
    <Button className="bg-pink-500 hover:bg-pink-600 text-white rounded-full px-8 py-4 text-lg shadow">
      dari cowokmu yang paling sayang kamu 💌
    </Button>
  </motion.div>
</main>

) }

