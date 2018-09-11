# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="de95b-101">тип перечисления defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="de95b-101">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="de95b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="de95b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de95b-103">Возможные значения уровня блокировки облака</span><span class="sxs-lookup"><span data-stu-id="de95b-103">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="de95b-104">Члены</span><span class="sxs-lookup"><span data-stu-id="de95b-104">Members</span></span>
|<span data-ttu-id="de95b-105">Член</span><span class="sxs-lookup"><span data-stu-id="de95b-105">Member</span></span>|<span data-ttu-id="de95b-106">Значение</span><span class="sxs-lookup"><span data-stu-id="de95b-106">Value</span></span>|<span data-ttu-id="de95b-107">Описание</span><span class="sxs-lookup"><span data-stu-id="de95b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de95b-108">notConfigured</span><span class="sxs-lookup"><span data-stu-id="de95b-108">notConfigured</span></span>|<span data-ttu-id="de95b-109">0</span><span class="sxs-lookup"><span data-stu-id="de95b-109">0%</span></span>|<span data-ttu-id="de95b-110">Значение по умолчанию, использует по умолчанию уровень блокировки антивирусной программы Защитник Windows и обеспечивает строгое обнаружение без увеличения риска для обнаружения допустимых файлов</span><span class="sxs-lookup"><span data-stu-id="de95b-110">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="de95b-111">high</span><span class="sxs-lookup"><span data-stu-id="de95b-111">High</span></span>|<span data-ttu-id="de95b-112">1</span><span class="sxs-lookup"><span data-stu-id="de95b-112">-1</span></span>|<span data-ttu-id="de95b-113">"High" применяет повышенный уровень обнаружения.</span><span class="sxs-lookup"><span data-stu-id="de95b-113">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="de95b-114">highPlus</span><span class="sxs-lookup"><span data-stu-id="de95b-114">highPlus</span></span>|<span data-ttu-id="de95b-115">2</span><span class="sxs-lookup"><span data-stu-id="de95b-115">2</span></span>|<span data-ttu-id="de95b-116">"High +" использует высокий уровень и применяет дополнительные средства защиты</span><span class="sxs-lookup"><span data-stu-id="de95b-116">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="de95b-117">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="de95b-117">zeroTolerance</span></span>|<span data-ttu-id="de95b-118">3</span><span class="sxs-lookup"><span data-stu-id="de95b-118">3</span></span>|<span data-ttu-id="de95b-119">"Zero tolerance" блокирует все неизвестные исполняемые файлы</span><span class="sxs-lookup"><span data-stu-id="de95b-119">Zero tolerance blocks all unknown executables</span></span>|








