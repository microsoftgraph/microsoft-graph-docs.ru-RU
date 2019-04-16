---
title: Клонирование команды
description: Создание копии команды. Эта операция также создает копию соответствующей группы.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1495e00e2332ce6b963e654b8f5d63b2882c778d
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2019
ms.locfileid: "31889963"
---
# <a name="clone-a-team"></a><span data-ttu-id="82c4c-104">Клонирование команды</span><span class="sxs-lookup"><span data-stu-id="82c4c-104">Clone a team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82c4c-105">Создание копии [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="82c4c-105">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="82c4c-106">Эта операция также создает копию соответствующей [группы](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="82c4c-106">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="82c4c-107">Вы можете указать, какие части команды необходимо клонировать:</span><span class="sxs-lookup"><span data-stu-id="82c4c-107">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="82c4c-108">**Apps** — копирует приложения Microsoft Teams, которые установлены в команде.</span><span class="sxs-lookup"><span data-stu-id="82c4c-108">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="82c4c-109">**channels** — копирует структуру канала (но не сообщения в канале).</span><span class="sxs-lookup"><span data-stu-id="82c4c-109">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="82c4c-110">**Members (участники** ) — копирует участников и владельцев группы.</span><span class="sxs-lookup"><span data-stu-id="82c4c-110">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="82c4c-111">**Settings** — копирует все параметры в группе, а также параметры группы ключей.</span><span class="sxs-lookup"><span data-stu-id="82c4c-111">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="82c4c-112">**вкладки** — копирует вкладки в каналах.</span><span class="sxs-lookup"><span data-stu-id="82c4c-112">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="82c4c-113">Когда вкладки клонированы, они помещаются в ненастроенное состояние, которые отображаются на панели вкладок в Microsoft Teams, и при первом их открытии вы увидите экран Конфигурация.</span><span class="sxs-lookup"><span data-stu-id="82c4c-113">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="82c4c-114">(Если пользователь, открывающий вкладку, не имеет разрешения на настройку приложений, они увидят сообщение о том, что вкладка еще не настроена.)</span><span class="sxs-lookup"><span data-stu-id="82c4c-114">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="82c4c-115">Клонирование является длительной операцией.</span><span class="sxs-lookup"><span data-stu-id="82c4c-115">Cloning is a long-running operation.</span></span>
<span data-ttu-id="82c4c-116">После возврата клона POST необходимо получить [операцию](../resources/teamsasyncoperation.md) , чтобы убедиться, что он "работает" или "выполнено" или "Failed".</span><span class="sxs-lookup"><span data-stu-id="82c4c-116">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="82c4c-117">Вы должны продолжать работу, пока не запустятся состояние "работает".</span><span class="sxs-lookup"><span data-stu-id="82c4c-117">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="82c4c-118">Рекомендуемая задержка между возвратами составляет 5 секунд.</span><span class="sxs-lookup"><span data-stu-id="82c4c-118">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="82c4c-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82c4c-119">Permissions</span></span>

<span data-ttu-id="82c4c-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82c4c-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82c4c-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82c4c-122">Permission type</span></span>      | <span data-ttu-id="82c4c-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82c4c-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82c4c-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82c4c-124">Delegated (work or school account)</span></span>     | <span data-ttu-id="82c4c-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82c4c-125">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="82c4c-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82c4c-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82c4c-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82c4c-127">Not supported.</span></span>    |
|<span data-ttu-id="82c4c-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82c4c-128">Application</span></span>                            | <span data-ttu-id="82c4c-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82c4c-129">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="82c4c-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82c4c-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="82c4c-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82c4c-131">Request headers</span></span>
| <span data-ttu-id="82c4c-132">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82c4c-132">Header</span></span>       | <span data-ttu-id="82c4c-133">Значение</span><span class="sxs-lookup"><span data-stu-id="82c4c-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="82c4c-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82c4c-134">Authorization</span></span>  | <span data-ttu-id="82c4c-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82c4c-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="82c4c-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="82c4c-137">Content-Type</span></span>  | <span data-ttu-id="82c4c-138">application/json</span><span class="sxs-lookup"><span data-stu-id="82c4c-138">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="82c4c-139">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="82c4c-139">Request body</span></span>

| <span data-ttu-id="82c4c-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="82c4c-140">Property</span></span>     | <span data-ttu-id="82c4c-141">Тип</span><span class="sxs-lookup"><span data-stu-id="82c4c-141">Type</span></span>   |<span data-ttu-id="82c4c-142">Описание</span><span class="sxs-lookup"><span data-stu-id="82c4c-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82c4c-143">classification</span><span class="sxs-lookup"><span data-stu-id="82c4c-143">classification</span></span>|<span data-ttu-id="82c4c-144">Строка (необязательно)</span><span class="sxs-lookup"><span data-stu-id="82c4c-144">String (optional)</span></span>|<span data-ttu-id="82c4c-145">Описывает классификацию для группы (например, снижение, среднее или высокое влияние на бизнес).</span><span class="sxs-lookup"><span data-stu-id="82c4c-145">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="82c4c-146">Допустимые значения для этого свойства определяются путем создания значения [параметра](../resources/directorysetting.md) классификатионлист на основе [определения шаблона](../resources/directorysettingtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="82c4c-146">Valid values for this property are defined by creating a ClassificationList [setting](../resources/directorysetting.md) value, based on the [template definition](../resources/directorysettingtemplate.md).</span></span> <span data-ttu-id="82c4c-147">Если классификация не указана, то классификация будет скопирована из исходной группы или группы.</span><span class="sxs-lookup"><span data-stu-id="82c4c-147">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="82c4c-148">description</span><span class="sxs-lookup"><span data-stu-id="82c4c-148">description</span></span>|<span data-ttu-id="82c4c-149">Строка (необязательно)</span><span class="sxs-lookup"><span data-stu-id="82c4c-149">String (optional)</span></span>|<span data-ttu-id="82c4c-150">Необязательное описание для группы.</span><span class="sxs-lookup"><span data-stu-id="82c4c-150">An optional description for the group.</span></span> <span data-ttu-id="82c4c-151">Если это свойство не задано, оно будет оставлено пустым.</span><span class="sxs-lookup"><span data-stu-id="82c4c-151">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="82c4c-152">displayName</span><span class="sxs-lookup"><span data-stu-id="82c4c-152">displayName</span></span>|<span data-ttu-id="82c4c-153">String</span><span class="sxs-lookup"><span data-stu-id="82c4c-153">String</span></span>|<span data-ttu-id="82c4c-p109">Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления. Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="82c4c-p109">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="82c4c-157">mailNickname</span><span class="sxs-lookup"><span data-stu-id="82c4c-157">mailNickname</span></span>|<span data-ttu-id="82c4c-158">String</span><span class="sxs-lookup"><span data-stu-id="82c4c-158">String</span></span>|<span data-ttu-id="82c4c-159">Почтовый псевдоним для группы (уникальный в организации).</span><span class="sxs-lookup"><span data-stu-id="82c4c-159">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="82c4c-160">Это свойство должно быть указано при создании группы.</span><span class="sxs-lookup"><span data-stu-id="82c4c-160">This property must be specified when a group is created.</span></span> <span data-ttu-id="82c4c-161">Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="82c4c-161">Supports $filter.</span></span> <span data-ttu-id="82c4c-162">Если это свойство не задано, оно будет вычислено в displayName.</span><span class="sxs-lookup"><span data-stu-id="82c4c-162">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="82c4c-163">Известная проблема: данное свойство в настоящее время игнорируется.</span><span class="sxs-lookup"><span data-stu-id="82c4c-163">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="82c4c-164">Партстоклоне</span><span class="sxs-lookup"><span data-stu-id="82c4c-164">partsToClone</span></span>| [<span data-ttu-id="82c4c-165">Клонаблетеампартс</span><span class="sxs-lookup"><span data-stu-id="82c4c-165">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="82c4c-166">Разделенный запятыми список частей, которые необходимо клонировать.</span><span class="sxs-lookup"><span data-stu-id="82c4c-166">A comma-separated list of the parts to clone.</span></span> <span data-ttu-id="82c4c-167">Юридическими частями являются "приложения, вкладки, параметры, каналы, элементы".</span><span class="sxs-lookup"><span data-stu-id="82c4c-167">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="82c4c-168">visibility</span><span class="sxs-lookup"><span data-stu-id="82c4c-168">visibility</span></span>|<span data-ttu-id="82c4c-169">[объекта teamvisibilitytype](../resources/teamvisibilitytype.md) необязательно</span><span class="sxs-lookup"><span data-stu-id="82c4c-169">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span></span>| <span data-ttu-id="82c4c-170">Задает видимость группы.</span><span class="sxs-lookup"><span data-stu-id="82c4c-170">Specifies the visibility of the group.</span></span> <span data-ttu-id="82c4c-171">Возможные значения: **Private**, **Public**.</span><span class="sxs-lookup"><span data-stu-id="82c4c-171">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="82c4c-172">Если параметр Visibility не указан, то видимость будет скопирована из исходной группы или группы.</span><span class="sxs-lookup"><span data-stu-id="82c4c-172">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="82c4c-173">Если группа является клонированной, параметр видимости \*\*\*\* игнорируется, и для отображения новой группы будет задано значение значение hiddenmembership.</span><span class="sxs-lookup"><span data-stu-id="82c4c-173">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="82c4c-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="82c4c-174">Response</span></span>

<span data-ttu-id="82c4c-175">В случае успеха этот метод возвратит код `202 Accepted` отклика с расположением: Header, указывающий на ресурс [Operation](../resources/teamsasyncoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="82c4c-175">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="82c4c-176">После завершения операции ресурс Operation сообщит вам идентификатор созданной команды.</span><span class="sxs-lookup"><span data-stu-id="82c4c-176">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="82c4c-177">Пример</span><span class="sxs-lookup"><span data-stu-id="82c4c-177">Example</span></span>
#### <a name="request"></a><span data-ttu-id="82c4c-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="82c4c-178">Request</span></span>
<span data-ttu-id="82c4c-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82c4c-179">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="82c4c-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="82c4c-180">Response</span></span>
<span data-ttu-id="82c4c-181">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="82c4c-181">The following is an example of the response.</span></span> <span data-ttu-id="82c4c-182">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="82c4c-182">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="82c4c-183">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82c4c-183">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
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
