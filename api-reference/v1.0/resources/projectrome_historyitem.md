# <a name="historyitem-resource-type"></a><span data-ttu-id="701a3-101">Тип ресурса historyItem</span><span class="sxs-lookup"><span data-stu-id="701a3-101">historyItem resource type</span></span>

<span data-ttu-id="701a3-102">Представляет элемент журнала для [действия](projectrome_activity.md) в приложении.</span><span class="sxs-lookup"><span data-stu-id="701a3-102">Represents a history item for an [activity](projectrome_activity.md) in an app.</span></span> <span data-ttu-id="701a3-103">Действия пользователя представляют собой отдельный пункт назначения в вашем приложении - например, телешоу, документ или текущую кампанию в видеоигре.</span><span class="sxs-lookup"><span data-stu-id="701a3-103">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="701a3-104">Когда пользователь подключает это действие, это задействование регистрируется как элемент журнала, указывающий время начала и окончания для этого действия.</span><span class="sxs-lookup"><span data-stu-id="701a3-104">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="701a3-105">По мере того как пользователь повторно подключает это действие с течением времени, в журнал записывается несколько элементов для одного действия пользователя.</span><span class="sxs-lookup"><span data-stu-id="701a3-105">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="701a3-106">Когда приложение создает сеанс, объект **historyItem** следует добавить к объекту **activity**, чтобы отразить период задействования пользователя.</span><span class="sxs-lookup"><span data-stu-id="701a3-106">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="701a3-107">При каждом следующем взаимодействии пользователя с действием, к действию добавляется новый элемент **historyItem** для контроля задействования пользователя.</span><span class="sxs-lookup"><span data-stu-id="701a3-107">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="701a3-108">Методы</span><span class="sxs-lookup"><span data-stu-id="701a3-108">Methods</span></span>

|<span data-ttu-id="701a3-109">Метод</span><span class="sxs-lookup"><span data-stu-id="701a3-109">Method</span></span> | <span data-ttu-id="701a3-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="701a3-110">Return Type</span></span> | <span data-ttu-id="701a3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="701a3-111">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="701a3-112">Создать или заменить historyItem</span><span class="sxs-lookup"><span data-stu-id="701a3-112">Create or replace historyItem</span></span>](../api/projectrome_put_historyitem.md) | <span data-ttu-id="701a3-113">[historyItem](projectrome_historyitem.md)</span><span class="sxs-lookup"><span data-stu-id="701a3-113">Added [historyItem](projectrome_historyitem.md)</span></span> | <span data-ttu-id="701a3-114">Создает или заменяет существующий **historyItem** для этого действия (обновление или вставка).</span><span class="sxs-lookup"><span data-stu-id="701a3-114">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="701a3-115"> ID должен быть идентификатором GUID.</span><span class="sxs-lookup"><span data-stu-id="701a3-115">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="701a3-116">Удалить historyItem</span><span class="sxs-lookup"><span data-stu-id="701a3-116">Delete a historyItem</span></span>](../api/projectrome_delete_historyitem.md) | <span data-ttu-id="701a3-117">Нет содержимого</span><span class="sxs-lookup"><span data-stu-id="701a3-117">204 No Content</span></span> | <span data-ttu-id="701a3-118">Удаляет указанный **historyItem** для этого действия.</span><span class="sxs-lookup"><span data-stu-id="701a3-118">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="701a3-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="701a3-119">Properties</span></span>

|<span data-ttu-id="701a3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="701a3-120">Name</span></span> | <span data-ttu-id="701a3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="701a3-121">Type</span></span> | <span data-ttu-id="701a3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="701a3-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="701a3-123">status</span><span class="sxs-lookup"><span data-stu-id="701a3-123">status</span></span> | <span data-ttu-id="701a3-124">status</span><span class="sxs-lookup"><span data-stu-id="701a3-124">status</span></span> | <span data-ttu-id="701a3-125">Устанавливается сервером.</span><span class="sxs-lookup"><span data-stu-id="701a3-125">Set by the server.</span></span> <span data-ttu-id="701a3-126">Код состояния, используемый для идентификации допустимых объектов.</span><span class="sxs-lookup"><span data-stu-id="701a3-126">A status code used to identify valid objects.</span></span> <span data-ttu-id="701a3-127">Значения: активный, обновлён, удалён, игнорируется.</span><span class="sxs-lookup"><span data-stu-id="701a3-127">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="701a3-128">userTimezone</span><span class="sxs-lookup"><span data-stu-id="701a3-128">userTimezone</span></span> | <span data-ttu-id="701a3-129">String</span><span class="sxs-lookup"><span data-stu-id="701a3-129">String</span></span> | <span data-ttu-id="701a3-130">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="701a3-130">Optional.</span></span> <span data-ttu-id="701a3-131">Часовой пояс, в котором устройство пользователя, используемое для создания действия, находилось во время создания действия.</span><span class="sxs-lookup"><span data-stu-id="701a3-131">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="701a3-132">Значения, представленные как Олсон-идентификаторы для поддержки кросс-платформенного представления.</span><span class="sxs-lookup"><span data-stu-id="701a3-132">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="701a3-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="701a3-133">createdDateTime</span></span> | <span data-ttu-id="701a3-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="701a3-134">DateTimeOffset</span></span> | <span data-ttu-id="701a3-135">Устанавливается сервером.</span><span class="sxs-lookup"><span data-stu-id="701a3-135">Set by the server.</span></span> <span data-ttu-id="701a3-136">Дата и время создания объекта на сервере в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="701a3-136">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="701a3-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="701a3-137">lastModifiedDateTime</span></span> | <span data-ttu-id="701a3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="701a3-138">DateTimeOffset</span></span> | <span data-ttu-id="701a3-139">Устанавливается сервером.</span><span class="sxs-lookup"><span data-stu-id="701a3-139">Set by the server.</span></span> <span data-ttu-id="701a3-140">Дата и время изменения объекта на сервере в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="701a3-140">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="701a3-141">id</span><span class="sxs-lookup"><span data-stu-id="701a3-141">id</span></span> | <span data-ttu-id="701a3-142">Строка</span><span class="sxs-lookup"><span data-stu-id="701a3-142">String</span></span> | <span data-ttu-id="701a3-143">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="701a3-143">Required.</span></span> <span data-ttu-id="701a3-144">Идентификатор GUID набора клиента для объекта **historyItem**.</span><span class="sxs-lookup"><span data-stu-id="701a3-144">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="701a3-145">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="701a3-145">startedDateTime</span></span> | <span data-ttu-id="701a3-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="701a3-146">DateTimeOffset</span></span> | <span data-ttu-id="701a3-147">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="701a3-147">Required.</span></span> <span data-ttu-id="701a3-148">Дата и время в формате UTC запуска **historyItem** (сеанса действия).</span><span class="sxs-lookup"><span data-stu-id="701a3-148">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="701a3-149">Требуется для журнала временной шкалы.</span><span class="sxs-lookup"><span data-stu-id="701a3-149">Required for timeline history.</span></span>|
|<span data-ttu-id="701a3-150">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="701a3-150">lastActiveDateTime</span></span> | <span data-ttu-id="701a3-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="701a3-151">DateTimeOffset</span></span> | <span data-ttu-id="701a3-152">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="701a3-152">Optional.</span></span> <span data-ttu-id="701a3-153">Дата и время в формате UTC, когда **historyItem** (сеанс действия) в последний раз считался активным или законченным. Если значение null, статус **historyItem** должен быть Ongoing.</span><span class="sxs-lookup"><span data-stu-id="701a3-153">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="701a3-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="701a3-154">expirationDateTime</span></span> | <span data-ttu-id="701a3-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="701a3-155">DateTimeOffset</span></span> | <span data-ttu-id="701a3-156">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="701a3-156">Optional.</span></span> <span data-ttu-id="701a3-157">Дата и время в формате UTC, когда **historyItem** будет окончательно удален.</span><span class="sxs-lookup"><span data-stu-id="701a3-157">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="701a3-158">Может быть задано клиентом.</span><span class="sxs-lookup"><span data-stu-id="701a3-158">Can be set by the client.</span></span>|
|<span data-ttu-id="701a3-159">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="701a3-159">activeDurationSeconds</span></span> | <span data-ttu-id="701a3-160">int</span><span class="sxs-lookup"><span data-stu-id="701a3-160">int</span></span> | <span data-ttu-id="701a3-161">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="701a3-161">Optional.</span></span> <span data-ttu-id="701a3-162">Длительность задействования активного пользователя.</span><span class="sxs-lookup"><span data-stu-id="701a3-162">The duration of active user engagement.</span></span> <span data-ttu-id="701a3-163">Если не указано, вычисляется по **startedDateTime** и **lastActiveDateTime**.</span><span class="sxs-lookup"><span data-stu-id="701a3-163">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="701a3-164">Связи</span><span class="sxs-lookup"><span data-stu-id="701a3-164">Relationships</span></span>

|<span data-ttu-id="701a3-165">Связь</span><span class="sxs-lookup"><span data-stu-id="701a3-165">Relationship</span></span> | <span data-ttu-id="701a3-166">Тип</span><span class="sxs-lookup"><span data-stu-id="701a3-166">Type</span></span> | <span data-ttu-id="701a3-167">Описание</span><span class="sxs-lookup"><span data-stu-id="701a3-167">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="701a3-168">activity</span><span class="sxs-lookup"><span data-stu-id="701a3-168">activity</span></span>| [<span data-ttu-id="701a3-169">userActivity</span><span class="sxs-lookup"><span data-stu-id="701a3-169">userActivity</span></span>](../resources/projectrome_activity.md) | <span data-ttu-id="701a3-170">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="701a3-170">Optional.</span></span> <span data-ttu-id="701a3-171">NavigationProperty/Containment; свойство навигации для связанного действия.</span><span class="sxs-lookup"><span data-stu-id="701a3-171">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="701a3-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="701a3-172">JSON representation</span></span>

<span data-ttu-id="701a3-173">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="701a3-173">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.activityHistoryItem",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
    "status": "active | updated | deleted | ignored",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "id": "String",
    "expirationDateTime": "DateTimeOffset",
    "startedDateTime": "DateTimeOffset",
    "userTimezone": "String",
    "lastActiveDateTime": "DateTimeOffset",
    "activeDurationSeconds":"int"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
