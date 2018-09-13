# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="f853e-101">Тип перечисления safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="f853e-101">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="f853e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f853e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f853e-103">Указывает, какой уровень безопасности поиска (фильтрация содержимого для взрослых) является обязательным</span><span class="sxs-lookup"><span data-stu-id="f853e-103">Specifies what filter level of safe search is required.</span></span>
## <a name="members"></a><span data-ttu-id="f853e-104">Элементы</span><span class="sxs-lookup"><span data-stu-id="f853e-104">Members</span></span>
|<span data-ttu-id="f853e-105">Элемент</span><span class="sxs-lookup"><span data-stu-id="f853e-105">Member</span></span>|<span data-ttu-id="f853e-106">Значение</span><span class="sxs-lookup"><span data-stu-id="f853e-106">Value</span></span>|<span data-ttu-id="f853e-107">Описание</span><span class="sxs-lookup"><span data-stu-id="f853e-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f853e-108">userDefined</span><span class="sxs-lookup"><span data-stu-id="f853e-108">userDefined</span></span>|<span data-ttu-id="f853e-109">0</span><span class="sxs-lookup"><span data-stu-id="f853e-109">0%</span></span>|<span data-ttu-id="f853e-110">Определено пользователем, значение по умолчанию, без назначения.</span><span class="sxs-lookup"><span data-stu-id="f853e-110">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="f853e-111">strict</span><span class="sxs-lookup"><span data-stu-id="f853e-111">Strict:</span></span>|<span data-ttu-id="f853e-112">1</span><span class="sxs-lookup"><span data-stu-id="f853e-112">-1</span></span>|<span data-ttu-id="f853e-113">Строгий, максимальная фильтрация содержимого для взрослых.</span><span class="sxs-lookup"><span data-stu-id="f853e-113">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="f853e-114">moderate</span><span class="sxs-lookup"><span data-stu-id="f853e-114">Moderate</span></span>|<span data-ttu-id="f853e-115">2</span><span class="sxs-lookup"><span data-stu-id="f853e-115">2</span></span>|<span data-ttu-id="f853e-116">Средняя фильтрация содержимого для взрослых (допустимые результаты поиска не будут фильтроваться).</span><span class="sxs-lookup"><span data-stu-id="f853e-116">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|








