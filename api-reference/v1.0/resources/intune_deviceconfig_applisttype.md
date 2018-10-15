# <a name="applisttype-enum-type"></a><span data-ttu-id="a0719-101">тип перечисления appListType</span><span class="sxs-lookup"><span data-stu-id="a0719-101">appListType enum type</span></span>

> <span data-ttu-id="a0719-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a0719-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0719-103">Возможные значения списка приложений на соответствие требованиям.</span><span class="sxs-lookup"><span data-stu-id="a0719-103">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="a0719-104">Элементы</span><span class="sxs-lookup"><span data-stu-id="a0719-104">Members</span></span>
|<span data-ttu-id="a0719-105">Элемент</span><span class="sxs-lookup"><span data-stu-id="a0719-105">Member</span></span>|<span data-ttu-id="a0719-106">Значение</span><span class="sxs-lookup"><span data-stu-id="a0719-106">Value</span></span>|<span data-ttu-id="a0719-107">Описание</span><span class="sxs-lookup"><span data-stu-id="a0719-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0719-108">none</span><span class="sxs-lookup"><span data-stu-id="a0719-108">none</span></span>|<span data-ttu-id="a0719-109">0</span><span class="sxs-lookup"><span data-stu-id="a0719-109">0%</span></span>|<span data-ttu-id="a0719-110">Значение по умолчанию, без назначения.</span><span class="sxs-lookup"><span data-stu-id="a0719-110">Default value, no intent.</span></span>|
|<span data-ttu-id="a0719-111">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="a0719-111">appsInListCompliant</span></span>|<span data-ttu-id="a0719-112">1</span><span class="sxs-lookup"><span data-stu-id="a0719-112">-1</span></span>|<span data-ttu-id="a0719-113">Список представляет приложения, которые будут считаться соответствующими требованиям (только приложения в списке соответствуют требованиям).</span><span class="sxs-lookup"><span data-stu-id="a0719-113">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="a0719-114">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="a0719-114">appsNotInListCompliant</span></span>|<span data-ttu-id="a0719-115">2</span><span class="sxs-lookup"><span data-stu-id="a0719-115">2</span></span>|<span data-ttu-id="a0719-116">Список представляет приложения, которые будут считаться несоответствующими требованиям (все приложения соответствуют требованиям, кроме перечисленных в списке).</span><span class="sxs-lookup"><span data-stu-id="a0719-116">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|








