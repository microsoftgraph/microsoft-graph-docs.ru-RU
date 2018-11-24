# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="3d06e-101">Тип ресурса teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="3d06e-101">teamsAppInstallation resource type</span></span>



<span data-ttu-id="3d06e-102">[TeamsApp](teamsapp.md) установлен в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="3d06e-102">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="3d06e-103">Любой программы-роботы, являющихся частью приложения становится частью любой группы добавляется приложение.</span><span class="sxs-lookup"><span data-stu-id="3d06e-103">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="3d06e-104">Методы</span><span class="sxs-lookup"><span data-stu-id="3d06e-104">Methods</span></span>

| <span data-ttu-id="3d06e-105">Метод</span><span class="sxs-lookup"><span data-stu-id="3d06e-105">Method</span></span>       | <span data-ttu-id="3d06e-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3d06e-106">Return Type</span></span>  |<span data-ttu-id="3d06e-107">Описание</span><span class="sxs-lookup"><span data-stu-id="3d06e-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3d06e-108">Список приложений</span><span class="sxs-lookup"><span data-stu-id="3d06e-108">List apps</span></span>](../api/teamsappinstallation_list.md) | [<span data-ttu-id="3d06e-109">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="3d06e-109">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="3d06e-110">Список приложений, установленные в группе.</span><span class="sxs-lookup"><span data-stu-id="3d06e-110">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="3d06e-111">Добавить приложение</span><span class="sxs-lookup"><span data-stu-id="3d06e-111">Add app</span></span>](../api/teamsappinstallation_add.md) | [<span data-ttu-id="3d06e-112">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="3d06e-112">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="3d06e-113">Добавляет (установить) приложения в группу.</span><span class="sxs-lookup"><span data-stu-id="3d06e-113">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="3d06e-114">Удаление приложения</span><span class="sxs-lookup"><span data-stu-id="3d06e-114">Remove app</span></span>](../api/teamsappinstallation_delete.md) | <span data-ttu-id="3d06e-115">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="3d06e-115">None</span></span> | <span data-ttu-id="3d06e-116">Удаляет (удаление) приложения из группы.</span><span class="sxs-lookup"><span data-stu-id="3d06e-116">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="3d06e-117">Обновление приложения</span><span class="sxs-lookup"><span data-stu-id="3d06e-117">Upgrade app</span></span>](../api/teamsappinstallation_delete.md) | <span data-ttu-id="3d06e-118">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="3d06e-118">None</span></span> | <span data-ttu-id="3d06e-119">Обновление до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="3d06e-119">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="3d06e-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d06e-120">Properties</span></span>

| <span data-ttu-id="3d06e-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d06e-121">Property</span></span>            | <span data-ttu-id="3d06e-122">Тип</span><span class="sxs-lookup"><span data-stu-id="3d06e-122">Type</span></span>     | <span data-ttu-id="3d06e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3d06e-123">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="3d06e-124">id</span><span class="sxs-lookup"><span data-stu-id="3d06e-124">id</span></span>                  | <span data-ttu-id="3d06e-125">строка</span><span class="sxs-lookup"><span data-stu-id="3d06e-125">string</span></span>   | <span data-ttu-id="3d06e-126">Уникальный идентификатор (не appid команды).</span><span class="sxs-lookup"><span data-stu-id="3d06e-126">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="3d06e-127">Связи</span><span class="sxs-lookup"><span data-stu-id="3d06e-127">Relationships</span></span>

| <span data-ttu-id="3d06e-128">Связь</span><span class="sxs-lookup"><span data-stu-id="3d06e-128">Relationship</span></span>   | <span data-ttu-id="3d06e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3d06e-129">Type</span></span>    | <span data-ttu-id="3d06e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3d06e-130">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3d06e-131">teamsApp</span><span class="sxs-lookup"><span data-stu-id="3d06e-131">teamsApp</span></span>|[<span data-ttu-id="3d06e-132">teamsApp</span><span class="sxs-lookup"><span data-stu-id="3d06e-132">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="3d06e-133">Приложения, которая устанавливается.</span><span class="sxs-lookup"><span data-stu-id="3d06e-133">The app that is installed.</span></span> |
|<span data-ttu-id="3d06e-134">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="3d06e-134">teamsAppDefinition</span></span>|[<span data-ttu-id="3d06e-135">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="3d06e-135">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="3d06e-136">Подробные сведения о данной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="3d06e-136">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3d06e-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3d06e-137">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
}
```

# <a name="see-also"></a><span data-ttu-id="3d06e-138">См. также</span><span class="sxs-lookup"><span data-stu-id="3d06e-138">See also</span></span>

- [<span data-ttu-id="3d06e-139">teamsApp</span><span class="sxs-lookup"><span data-stu-id="3d06e-139">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="3d06e-140">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="3d06e-140">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="3d06e-141">teamsTab</span><span class="sxs-lookup"><span data-stu-id="3d06e-141">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

