# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="a3df7-101">тип перечисления sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="a3df7-101">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="a3df7-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a3df7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3df7-103">Возможные значения при удалении учетных записей на общем ПК.</span><span class="sxs-lookup"><span data-stu-id="a3df7-103">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="a3df7-104">Элементы</span><span class="sxs-lookup"><span data-stu-id="a3df7-104">Members</span></span>
|<span data-ttu-id="a3df7-105">Элемент</span><span class="sxs-lookup"><span data-stu-id="a3df7-105">Member</span></span>|<span data-ttu-id="a3df7-106">Значение</span><span class="sxs-lookup"><span data-stu-id="a3df7-106">Value</span></span>|<span data-ttu-id="a3df7-107">Описание</span><span class="sxs-lookup"><span data-stu-id="a3df7-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3df7-108">immediate</span><span class="sxs-lookup"><span data-stu-id="a3df7-108">   [-immediate]</span></span>|<span data-ttu-id="a3df7-109">0</span><span class="sxs-lookup"><span data-stu-id="a3df7-109">0%</span></span>|<span data-ttu-id="a3df7-110">Немедленное удаление.</span><span class="sxs-lookup"><span data-stu-id="a3df7-110">Delete immediately.</span></span>|
|<span data-ttu-id="a3df7-111">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="a3df7-111">diskSpaceThreshold</span></span>|<span data-ttu-id="a3df7-112">1</span><span class="sxs-lookup"><span data-stu-id="a3df7-112">-1</span></span>|<span data-ttu-id="a3df7-113">Удаление у порога дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="a3df7-113">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="a3df7-114">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="a3df7-114">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="a3df7-115">2</span><span class="sxs-lookup"><span data-stu-id="a3df7-115">2</span></span>|<span data-ttu-id="a3df7-116">Удаление у порога дискового пространства или неактивного порога.</span><span class="sxs-lookup"><span data-stu-id="a3df7-116">Delete at disk space threshold or inactive threshold.</span></span>|








