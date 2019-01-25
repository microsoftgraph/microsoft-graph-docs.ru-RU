---
title: Клонирование группы
description: Создайте копию группы. Эта операция также создает копию соответствующей группе.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 5ef317d004e3355f9b40fc44232b7c594a3e45a7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526167"
---
# <a name="clone-a-team"></a><span data-ttu-id="bc9b8-104">Клонирование группы</span><span class="sxs-lookup"><span data-stu-id="bc9b8-104">Clone a team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc9b8-105">Создайте копию [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="bc9b8-105">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="bc9b8-106">Эта операция также создает копию в соответствующие [группы](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="bc9b8-106">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="bc9b8-107">Можно определить какие части группы следует скопировать.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-107">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="bc9b8-108">**приложения** - группами Майкрософт копий приложений, установленных в группе.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-108">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="bc9b8-109">**каналы** — копирует структуру канала (но не сообщения в канале).</span><span class="sxs-lookup"><span data-stu-id="bc9b8-109">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="bc9b8-110">**члены** — копирует участников и владельцев группы.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-110">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="bc9b8-111">**Параметры** — копирует все параметры в рамках рабочей группы, а также параметры ключа группы.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-111">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="bc9b8-112">**вкладки** — копирует вкладок между каналами.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-112">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="bc9b8-113">При клонировании вкладок они помещаются в исходное состояние — они отображаются в панели вкладок в группах Microsoft и при первом открытии, вы перейдете через экрана конфигурации.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-113">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="bc9b8-114">(Если пользователь на вкладке не имеет разрешения для настройки приложения, они появится сообщение о том, что вкладке еще не были настроены.)</span><span class="sxs-lookup"><span data-stu-id="bc9b8-114">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="bc9b8-115">Клонирование — это длительная операция.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-115">Cloning is a long-running operation.</span></span>
<span data-ttu-id="bc9b8-116">После возвращает клонированной POST, необходимо получить [операция](../resources/teamsasyncoperation.md) , является ли он «запуск» или «успешно» и «failed».</span><span class="sxs-lookup"><span data-stu-id="bc9b8-116">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="bc9b8-117">Следует продолжить GET, пока состояние не «выполняется».</span><span class="sxs-lookup"><span data-stu-id="bc9b8-117">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="bc9b8-118">Рекомендуемые задержки между получает — 5 секунд.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-118">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc9b8-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc9b8-119">Permissions</span></span>

<span data-ttu-id="bc9b8-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc9b8-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc9b8-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc9b8-122">Permission type</span></span>      | <span data-ttu-id="bc9b8-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc9b8-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc9b8-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc9b8-124">Delegated (work or school account)</span></span>     | <span data-ttu-id="bc9b8-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc9b8-125">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bc9b8-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc9b8-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc9b8-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-127">Not supported.</span></span>    |
|<span data-ttu-id="bc9b8-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc9b8-128">Application</span></span>                            | <span data-ttu-id="bc9b8-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc9b8-129">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc9b8-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc9b8-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="bc9b8-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc9b8-131">Request headers</span></span>
| <span data-ttu-id="bc9b8-132">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc9b8-132">Header</span></span>       | <span data-ttu-id="bc9b8-133">Значение</span><span class="sxs-lookup"><span data-stu-id="bc9b8-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bc9b8-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bc9b8-134">Authorization</span></span>  | <span data-ttu-id="bc9b8-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bc9b8-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bc9b8-137">Content-Type</span></span>  | <span data-ttu-id="bc9b8-138">application/json</span><span class="sxs-lookup"><span data-stu-id="bc9b8-138">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bc9b8-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc9b8-139">Request body</span></span>

| <span data-ttu-id="bc9b8-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc9b8-140">Property</span></span>     | <span data-ttu-id="bc9b8-141">Тип</span><span class="sxs-lookup"><span data-stu-id="bc9b8-141">Type</span></span>   |<span data-ttu-id="bc9b8-142">Описание</span><span class="sxs-lookup"><span data-stu-id="bc9b8-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc9b8-143">classification</span><span class="sxs-lookup"><span data-stu-id="bc9b8-143">classification</span></span>|<span data-ttu-id="bc9b8-144">String (необязательно)</span><span class="sxs-lookup"><span data-stu-id="bc9b8-144">String (optional)</span></span>|<span data-ttu-id="bc9b8-145">Описание классификации для группы (например, низкий, средний или высокий для бизнеса).</span><span class="sxs-lookup"><span data-stu-id="bc9b8-145">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="bc9b8-146">Допустимые значения для этого свойства определены, создав значение [параметра](../resources/directorysetting.md) ClassificationList на основе [определения шаблона](../resources/directorysettingtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="bc9b8-146">Valid values for this property are defined by creating a ClassificationList [setting](../resources/directorysetting.md) value, based on the [template definition](../resources/directorysettingtemplate.md).</span></span> <span data-ttu-id="bc9b8-147">Если классификация не указан, классификации копируются из исходной группы или группы.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-147">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="bc9b8-148">description</span><span class="sxs-lookup"><span data-stu-id="bc9b8-148">description</span></span>|<span data-ttu-id="bc9b8-149">String (необязательно)</span><span class="sxs-lookup"><span data-stu-id="bc9b8-149">String (optional)</span></span>|<span data-ttu-id="bc9b8-150">Необязательное описание для группы.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-150">An optional description for the group.</span></span> <span data-ttu-id="bc9b8-151">Если это свойство не указан, он остается пустым.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-151">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="bc9b8-152">displayName</span><span class="sxs-lookup"><span data-stu-id="bc9b8-152">displayName</span></span>|<span data-ttu-id="bc9b8-153">Строка</span><span class="sxs-lookup"><span data-stu-id="bc9b8-153">String</span></span>|<span data-ttu-id="bc9b8-p109">Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления. Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-p109">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="bc9b8-157">mailNickname</span><span class="sxs-lookup"><span data-stu-id="bc9b8-157">mailNickname</span></span>|<span data-ttu-id="bc9b8-158">String</span><span class="sxs-lookup"><span data-stu-id="bc9b8-158">String</span></span>|<span data-ttu-id="bc9b8-159">Почтовый псевдоним для группы (уникальный в организации).</span><span class="sxs-lookup"><span data-stu-id="bc9b8-159">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="bc9b8-160">Это свойство должно быть указано при создании группы.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-160">This property must be specified when a group is created.</span></span> <span data-ttu-id="bc9b8-161">Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-161">Supports $filter.</span></span> <span data-ttu-id="bc9b8-162">Если это свойство не задано, его повторное вычисление из displayName.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-162">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="bc9b8-163">Известные проблемы: это свойство учитывается.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-163">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="bc9b8-164">partsToClone</span><span class="sxs-lookup"><span data-stu-id="bc9b8-164">partsToClone</span></span>| [<span data-ttu-id="bc9b8-165">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="bc9b8-165">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="bc9b8-166">Список разделенных запятой частей следует скопировать.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-166">A comma-seperated list of the parts to clone.</span></span> <span data-ttu-id="bc9b8-167">Юридические части, «приложений, вкладок, параметры, каналы, участники».</span><span class="sxs-lookup"><span data-stu-id="bc9b8-167">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="bc9b8-168">visibility</span><span class="sxs-lookup"><span data-stu-id="bc9b8-168">visibility</span></span>|<span data-ttu-id="bc9b8-169">[teamVisibilityType](../resources/teamvisibilitytype.md) (необязательно)</span><span class="sxs-lookup"><span data-stu-id="bc9b8-169">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span></span>| <span data-ttu-id="bc9b8-170">Определяет видимость группы.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-170">Specifies the visibility of the group.</span></span> <span data-ttu-id="bc9b8-171">Возможные значения: **частный**, **открытым**.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-171">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="bc9b8-172">Если видимости не указан, видимости копируются из исходной группы или группы.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-172">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="bc9b8-173">Если группа клонировании — это группа **educationClass** , параметр видимости игнорируется и видимости новой группы будут иметь значение HiddenMembership.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-173">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="bc9b8-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc9b8-174">Response</span></span>

<span data-ttu-id="bc9b8-175">Если успешно завершена, этот метод возвращает `202 Accepted` код ответа с расположением: заголовок, с указанием ресурсов [операции](../resources/teamsasyncoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="bc9b8-175">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="bc9b8-176">После завершения операции ресурсов операции сообщит вам, идентификатор созданного группы.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-176">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="bc9b8-177">Пример</span><span class="sxs-lookup"><span data-stu-id="bc9b8-177">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bc9b8-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc9b8-178">Request</span></span>
<span data-ttu-id="bc9b8-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-179">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="bc9b8-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc9b8-180">Response</span></span>
<span data-ttu-id="bc9b8-181">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-181">The following is an example of the response.</span></span> <span data-ttu-id="bc9b8-182">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-182">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bc9b8-183">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc9b8-183">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/team-clone.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
