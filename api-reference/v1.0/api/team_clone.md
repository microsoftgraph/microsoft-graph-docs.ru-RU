# <a name="clone-a-team"></a><span data-ttu-id="778cf-101">Клонирование группы</span><span class="sxs-lookup"><span data-stu-id="778cf-101">Clone a team</span></span>



<span data-ttu-id="778cf-102">Создайте копию [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="778cf-102">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="778cf-103">Эта операция также создает копию в соответствующие [группы](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="778cf-103">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="778cf-104">Можно определить какие части группы следует скопировать.</span><span class="sxs-lookup"><span data-stu-id="778cf-104">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="778cf-105">**приложения** - группами Майкрософт копий приложений, установленных в группе.</span><span class="sxs-lookup"><span data-stu-id="778cf-105">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="778cf-106">**каналы** — копирует структуру канала (но не сообщения в канале).</span><span class="sxs-lookup"><span data-stu-id="778cf-106">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="778cf-107">**члены** — копирует участников и владельцев группы.</span><span class="sxs-lookup"><span data-stu-id="778cf-107">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="778cf-108">**Параметры** — копирует все параметры в рамках рабочей группы, а также параметры ключа группы.</span><span class="sxs-lookup"><span data-stu-id="778cf-108">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="778cf-109">**вкладки** — копирует вкладок между каналами.</span><span class="sxs-lookup"><span data-stu-id="778cf-109">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="778cf-110">При клонировании вкладок они помещаются в исходное состояние — они отображаются в панели вкладок в группах Microsoft и при первом открытии, вы перейдете через экрана конфигурации.</span><span class="sxs-lookup"><span data-stu-id="778cf-110">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="778cf-111">(Если пользователь на вкладке не имеет разрешения для настройки приложения, они появится сообщение о том, что вкладке еще не были настроены.)</span><span class="sxs-lookup"><span data-stu-id="778cf-111">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="778cf-112">Клонирование — это длительная операция.</span><span class="sxs-lookup"><span data-stu-id="778cf-112">Cloning is a long-running operation.</span></span>
<span data-ttu-id="778cf-113">После возвращает клонированной POST, необходимо получить [операция](../resources/teamsasyncoperation.md) , является ли он «запуск» или «успешно» и «failed».</span><span class="sxs-lookup"><span data-stu-id="778cf-113">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="778cf-114">Следует продолжить GET, пока состояние не «выполняется».</span><span class="sxs-lookup"><span data-stu-id="778cf-114">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="778cf-115">Рекомендуемые задержки между получает — 5 секунд.</span><span class="sxs-lookup"><span data-stu-id="778cf-115">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="778cf-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="778cf-116">Permissions</span></span>

<span data-ttu-id="778cf-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="778cf-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="778cf-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="778cf-119">Permission type</span></span>      | <span data-ttu-id="778cf-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="778cf-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="778cf-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="778cf-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="778cf-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="778cf-122">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="778cf-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="778cf-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="778cf-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="778cf-124">Not supported.</span></span>    |
|<span data-ttu-id="778cf-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="778cf-125">Application</span></span>                            | <span data-ttu-id="778cf-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="778cf-126">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="778cf-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="778cf-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="778cf-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="778cf-128">Request headers</span></span>
| <span data-ttu-id="778cf-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="778cf-129">Header</span></span>       | <span data-ttu-id="778cf-130">Значение</span><span class="sxs-lookup"><span data-stu-id="778cf-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="778cf-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="778cf-131">Authorization</span></span>  | <span data-ttu-id="778cf-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="778cf-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="778cf-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="778cf-134">Content-Type</span></span>  | <span data-ttu-id="778cf-135">application/json</span><span class="sxs-lookup"><span data-stu-id="778cf-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="778cf-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="778cf-136">Request body</span></span>

| <span data-ttu-id="778cf-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="778cf-137">Property</span></span>     | <span data-ttu-id="778cf-138">Тип</span><span class="sxs-lookup"><span data-stu-id="778cf-138">Type</span></span>   |<span data-ttu-id="778cf-139">Описание</span><span class="sxs-lookup"><span data-stu-id="778cf-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="778cf-140">classification</span><span class="sxs-lookup"><span data-stu-id="778cf-140">classification</span></span>|<span data-ttu-id="778cf-141">String (необязательно)</span><span class="sxs-lookup"><span data-stu-id="778cf-141">String (optional)</span></span>|<span data-ttu-id="778cf-142">Описание классификации для группы (например, низкий, средний или высокий для бизнеса).</span><span class="sxs-lookup"><span data-stu-id="778cf-142">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="778cf-143">Если классификация не указан, классификации копируются из исходной группы или группы.</span><span class="sxs-lookup"><span data-stu-id="778cf-143">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="778cf-144">description</span><span class="sxs-lookup"><span data-stu-id="778cf-144">description</span></span>|<span data-ttu-id="778cf-145">String (необязательно)</span><span class="sxs-lookup"><span data-stu-id="778cf-145">String (optional)</span></span>|<span data-ttu-id="778cf-146">Необязательное описание для группы.</span><span class="sxs-lookup"><span data-stu-id="778cf-146">An optional description for the group.</span></span> <span data-ttu-id="778cf-147">Если это свойство не указан, он остается пустым.</span><span class="sxs-lookup"><span data-stu-id="778cf-147">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="778cf-148">displayName</span><span class="sxs-lookup"><span data-stu-id="778cf-148">displayName</span></span>|<span data-ttu-id="778cf-149">String</span><span class="sxs-lookup"><span data-stu-id="778cf-149">String</span></span>|<span data-ttu-id="778cf-p108">Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления. Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="778cf-p108">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="778cf-153">mailNickname</span><span class="sxs-lookup"><span data-stu-id="778cf-153">mailNickname</span></span>|<span data-ttu-id="778cf-154">String</span><span class="sxs-lookup"><span data-stu-id="778cf-154">String</span></span>|<span data-ttu-id="778cf-155">Псевдоним почты для группы, уникальные в организации.</span><span class="sxs-lookup"><span data-stu-id="778cf-155">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="778cf-156">Это свойство должен быть указан при создании группы.</span><span class="sxs-lookup"><span data-stu-id="778cf-156">This property must be specified when a group is created.</span></span> <span data-ttu-id="778cf-157">Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="778cf-157">Supports $filter.</span></span> <span data-ttu-id="778cf-158">Если это свойство не задано, его повторное вычисление из displayName.</span><span class="sxs-lookup"><span data-stu-id="778cf-158">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="778cf-159">Известные проблемы: это свойство учитывается.</span><span class="sxs-lookup"><span data-stu-id="778cf-159">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="778cf-160">partsToClone</span><span class="sxs-lookup"><span data-stu-id="778cf-160">partsToClone</span></span>| [<span data-ttu-id="778cf-161">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="778cf-161">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="778cf-162">Список разделенных запятой частей следует скопировать.</span><span class="sxs-lookup"><span data-stu-id="778cf-162">A comma-seperated list of the parts to clone.</span></span> <span data-ttu-id="778cf-163">Юридические части, «приложений, вкладок, параметры, каналы, участники».</span><span class="sxs-lookup"><span data-stu-id="778cf-163">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="778cf-164">visibility</span><span class="sxs-lookup"><span data-stu-id="778cf-164">visibility</span></span>|<span data-ttu-id="778cf-165">[teamVisibilityType](../resources/teamVisibilityType.md) (необязательно)</span><span class="sxs-lookup"><span data-stu-id="778cf-165">[teamVisibilityType](../resources/teamVisibilityType.md) (optional)</span></span>| <span data-ttu-id="778cf-166">Определяет видимость группы.</span><span class="sxs-lookup"><span data-stu-id="778cf-166">Specifies the visibility of the group.</span></span> <span data-ttu-id="778cf-167">Возможные значения: **частный**, **открытым**.</span><span class="sxs-lookup"><span data-stu-id="778cf-167">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="778cf-168">Если видимости не указан, видимости копируются из исходной группы или группы.</span><span class="sxs-lookup"><span data-stu-id="778cf-168">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="778cf-169">Если группа клонировании — это группа **educationClass** , параметр видимости игнорируется и видимости новой группы будут иметь значение HiddenMembership.</span><span class="sxs-lookup"><span data-stu-id="778cf-169">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="778cf-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="778cf-170">Response</span></span>

<span data-ttu-id="778cf-171">Если успешно завершена, этот метод возвращает `202 Accepted` код ответа с расположением: заголовок, с указанием ресурсов [операции](../resources/teamsasyncoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="778cf-171">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="778cf-172">После завершения операции ресурсов операции сообщит вам, идентификатор созданного группы.</span><span class="sxs-lookup"><span data-stu-id="778cf-172">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="778cf-173">Пример</span><span class="sxs-lookup"><span data-stu-id="778cf-173">Example</span></span>
#### <a name="request"></a><span data-ttu-id="778cf-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="778cf-174">Request</span></span>
<span data-ttu-id="778cf-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="778cf-175">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
POST /teams/{id}/clone
Content-Type: application/json

{  
     "displayName": "Library Assist",
     "description": "Self help community for library",
     "mailNickname": "libassist",
     "partsToClone": "apps,tabs,settings,channels,members",
     "visibility": "public"
}
```

#### <a name="response"></a><span data-ttu-id="778cf-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="778cf-176">Response</span></span>
<span data-ttu-id="778cf-177">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="778cf-177">The following is an example of the response.</span></span> <span data-ttu-id="778cf-178">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="778cf-178">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="778cf-179">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="778cf-179">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
