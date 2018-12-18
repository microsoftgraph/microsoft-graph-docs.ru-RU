---
title: Клонирование группы
description: Создайте копию группы. Эта операция также создает копию соответствующей группе.
author: nkramer
ms.openlocfilehash: 21671ccbe440a57f6d745f9587c09b4432e25c35
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321835"
---
# <a name="clone-a-team"></a><span data-ttu-id="16441-104">Клонирование группы</span><span class="sxs-lookup"><span data-stu-id="16441-104">Clone a team</span></span>



<span data-ttu-id="16441-105">Создайте копию [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="16441-105">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="16441-106">Эта операция также создает копию в соответствующие [группы](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="16441-106">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="16441-107">Можно определить какие части группы следует скопировать.</span><span class="sxs-lookup"><span data-stu-id="16441-107">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="16441-108">**приложения** - группами Майкрософт копий приложений, установленных в группе.</span><span class="sxs-lookup"><span data-stu-id="16441-108">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="16441-109">**каналы** — копирует структуру канала (но не сообщения в канале).</span><span class="sxs-lookup"><span data-stu-id="16441-109">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="16441-110">**члены** — копирует участников и владельцев группы.</span><span class="sxs-lookup"><span data-stu-id="16441-110">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="16441-111">**Параметры** — копирует все параметры в рамках рабочей группы, а также параметры ключа группы.</span><span class="sxs-lookup"><span data-stu-id="16441-111">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="16441-112">**вкладки** — копирует вкладок между каналами.</span><span class="sxs-lookup"><span data-stu-id="16441-112">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="16441-113">При клонировании вкладок они помещаются в исходное состояние — они отображаются в панели вкладок в группах Microsoft и при первом открытии, вы перейдете через экрана конфигурации.</span><span class="sxs-lookup"><span data-stu-id="16441-113">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="16441-114">(Если пользователь на вкладке не имеет разрешения для настройки приложения, они появится сообщение о том, что вкладке еще не были настроены.)</span><span class="sxs-lookup"><span data-stu-id="16441-114">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="16441-115">Клонирование — это длительная операция.</span><span class="sxs-lookup"><span data-stu-id="16441-115">Cloning is a long-running operation.</span></span>
<span data-ttu-id="16441-116">После возвращает клонированной POST, необходимо получить [операция](../resources/teamsasyncoperation.md) , является ли он «запуск» или «успешно» и «failed».</span><span class="sxs-lookup"><span data-stu-id="16441-116">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="16441-117">Следует продолжить GET, пока состояние не «выполняется».</span><span class="sxs-lookup"><span data-stu-id="16441-117">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="16441-118">Рекомендуемые задержки между получает — 5 секунд.</span><span class="sxs-lookup"><span data-stu-id="16441-118">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="16441-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16441-119">Permissions</span></span>

<span data-ttu-id="16441-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16441-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16441-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16441-122">Permission type</span></span>      | <span data-ttu-id="16441-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16441-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16441-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16441-124">Delegated (work or school account)</span></span>     | <span data-ttu-id="16441-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16441-125">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="16441-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16441-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16441-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16441-127">Not supported.</span></span>    |
|<span data-ttu-id="16441-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16441-128">Application</span></span>                            | <span data-ttu-id="16441-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16441-129">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16441-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16441-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="16441-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16441-131">Request headers</span></span>
| <span data-ttu-id="16441-132">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16441-132">Header</span></span>       | <span data-ttu-id="16441-133">Значение</span><span class="sxs-lookup"><span data-stu-id="16441-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="16441-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16441-134">Authorization</span></span>  | <span data-ttu-id="16441-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16441-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="16441-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="16441-137">Content-Type</span></span>  | <span data-ttu-id="16441-138">application/json</span><span class="sxs-lookup"><span data-stu-id="16441-138">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="16441-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16441-139">Request body</span></span>

| <span data-ttu-id="16441-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="16441-140">Property</span></span>     | <span data-ttu-id="16441-141">Тип</span><span class="sxs-lookup"><span data-stu-id="16441-141">Type</span></span>   |<span data-ttu-id="16441-142">Описание</span><span class="sxs-lookup"><span data-stu-id="16441-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16441-143">classification</span><span class="sxs-lookup"><span data-stu-id="16441-143">classification</span></span>|<span data-ttu-id="16441-144">String (необязательно)</span><span class="sxs-lookup"><span data-stu-id="16441-144">String (optional)</span></span>|<span data-ttu-id="16441-145">Описание классификации для группы (например, низкий, средний или высокий для бизнеса).</span><span class="sxs-lookup"><span data-stu-id="16441-145">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="16441-146">Если классификация не указан, классификации копируются из исходной группы или группы.</span><span class="sxs-lookup"><span data-stu-id="16441-146">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="16441-147">description</span><span class="sxs-lookup"><span data-stu-id="16441-147">description</span></span>|<span data-ttu-id="16441-148">String (необязательно)</span><span class="sxs-lookup"><span data-stu-id="16441-148">String (optional)</span></span>|<span data-ttu-id="16441-149">Необязательное описание для группы.</span><span class="sxs-lookup"><span data-stu-id="16441-149">An optional description for the group.</span></span> <span data-ttu-id="16441-150">Если это свойство не указан, он остается пустым.</span><span class="sxs-lookup"><span data-stu-id="16441-150">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="16441-151">displayName</span><span class="sxs-lookup"><span data-stu-id="16441-151">displayName</span></span>|<span data-ttu-id="16441-152">String</span><span class="sxs-lookup"><span data-stu-id="16441-152">String</span></span>|<span data-ttu-id="16441-p109">Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления. Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="16441-p109">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="16441-156">mailNickname</span><span class="sxs-lookup"><span data-stu-id="16441-156">mailNickname</span></span>|<span data-ttu-id="16441-157">String</span><span class="sxs-lookup"><span data-stu-id="16441-157">String</span></span>|<span data-ttu-id="16441-158">Псевдоним почты для группы, уникальные в организации.</span><span class="sxs-lookup"><span data-stu-id="16441-158">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="16441-159">Это свойство должен быть указан при создании группы.</span><span class="sxs-lookup"><span data-stu-id="16441-159">This property must be specified when a group is created.</span></span> <span data-ttu-id="16441-160">Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="16441-160">Supports $filter.</span></span> <span data-ttu-id="16441-161">Если это свойство не задано, его повторное вычисление из displayName.</span><span class="sxs-lookup"><span data-stu-id="16441-161">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="16441-162">Известные проблемы: это свойство учитывается.</span><span class="sxs-lookup"><span data-stu-id="16441-162">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="16441-163">partsToClone</span><span class="sxs-lookup"><span data-stu-id="16441-163">partsToClone</span></span>| [<span data-ttu-id="16441-164">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="16441-164">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="16441-165">Список разделенных запятой частей следует скопировать.</span><span class="sxs-lookup"><span data-stu-id="16441-165">A comma-seperated list of the parts to clone.</span></span> <span data-ttu-id="16441-166">Юридические части, «приложений, вкладок, параметры, каналы, участники».</span><span class="sxs-lookup"><span data-stu-id="16441-166">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="16441-167">visibility</span><span class="sxs-lookup"><span data-stu-id="16441-167">visibility</span></span>|<span data-ttu-id="16441-168">[teamVisibilityType](../resources/teamvisibilitytype.md) (необязательно)</span><span class="sxs-lookup"><span data-stu-id="16441-168">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span></span>| <span data-ttu-id="16441-169">Определяет видимость группы.</span><span class="sxs-lookup"><span data-stu-id="16441-169">Specifies the visibility of the group.</span></span> <span data-ttu-id="16441-170">Возможные значения: **частный**, **открытым**.</span><span class="sxs-lookup"><span data-stu-id="16441-170">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="16441-171">Если видимости не указан, видимости копируются из исходной группы или группы.</span><span class="sxs-lookup"><span data-stu-id="16441-171">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="16441-172">Если группа клонировании — это группа **educationClass** , параметр видимости игнорируется и видимости новой группы будут иметь значение HiddenMembership.</span><span class="sxs-lookup"><span data-stu-id="16441-172">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="16441-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="16441-173">Response</span></span>

<span data-ttu-id="16441-174">Если успешно завершена, этот метод возвращает `202 Accepted` код ответа с расположением: заголовок, с указанием ресурсов [операции](../resources/teamsasyncoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="16441-174">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="16441-175">После завершения операции ресурсов операции сообщит вам, идентификатор созданного группы.</span><span class="sxs-lookup"><span data-stu-id="16441-175">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="16441-176">Пример</span><span class="sxs-lookup"><span data-stu-id="16441-176">Example</span></span>
#### <a name="request"></a><span data-ttu-id="16441-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="16441-177">Request</span></span>
<span data-ttu-id="16441-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16441-178">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="16441-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="16441-179">Response</span></span>
<span data-ttu-id="16441-180">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="16441-180">The following is an example of the response.</span></span> <span data-ttu-id="16441-181">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="16441-181">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="16441-182">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16441-182">All of the properties will be returned from an actual call.</span></span>
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
