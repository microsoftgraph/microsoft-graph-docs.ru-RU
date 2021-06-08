---
title: Клонировать команду
description: Создайте копию команды. Эта операция также создает копию соответствующей группы.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6299d1e7ecf828ee6587c4a69796021f1905dfd5
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786862"
---
# <a name="clone-a-team"></a><span data-ttu-id="da9a5-104">Клонировать команду</span><span class="sxs-lookup"><span data-stu-id="da9a5-104">Clone a team</span></span>

<span data-ttu-id="da9a5-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da9a5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da9a5-106">Создайте копию [команды.](../resources/team.md)</span><span class="sxs-lookup"><span data-stu-id="da9a5-106">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="da9a5-107">Эта операция также создает копию соответствующей [группы.](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="da9a5-107">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="da9a5-108">Можно указать, какие части группы клонировать:</span><span class="sxs-lookup"><span data-stu-id="da9a5-108">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="da9a5-109">**приложения** — Microsoft Teams приложения, установленные в команде.</span><span class="sxs-lookup"><span data-stu-id="da9a5-109">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="da9a5-110">**каналы** — копирует структуру канала (но не сообщения в канале).</span><span class="sxs-lookup"><span data-stu-id="da9a5-110">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="da9a5-111">**члены** — копирует членов и владельцев группы.</span><span class="sxs-lookup"><span data-stu-id="da9a5-111">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="da9a5-112">**параметры** — копирует все параметры в команде, а также ключевые параметры группы.</span><span class="sxs-lookup"><span data-stu-id="da9a5-112">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="da9a5-113">**вкладки** — копирует вкладки в каналах.</span><span class="sxs-lookup"><span data-stu-id="da9a5-113">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="da9a5-114">Когда вкладки клонируют, они помещаются в неконфигурированное состояние — они отображаются на панели вкладок в Microsoft Teams, и при первом их открытие вы будете проходить через экран конфигурации.</span><span class="sxs-lookup"><span data-stu-id="da9a5-114">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="da9a5-115">(Если открывающий вкладку человек не имеет разрешения на настройку приложений, он увидит сообщение, объясняя, что вкладка не настроена.)</span><span class="sxs-lookup"><span data-stu-id="da9a5-115">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="da9a5-116">Клонирование является длительной операцией.</span><span class="sxs-lookup"><span data-stu-id="da9a5-116">Cloning is a long-running operation.</span></span>
<span data-ttu-id="da9a5-117">После возвращения клона POST необходимо получить [](../resources/teamsasyncoperation.md) операцию, возвращаемую расположением: заглавной, чтобы узнать, "запущена" или "успешно" или "не удалось".</span><span class="sxs-lookup"><span data-stu-id="da9a5-117">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) returned by the Location: header to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="da9a5-118">Вы должны продолжать получать, пока состояние не будет "запущено".</span><span class="sxs-lookup"><span data-stu-id="da9a5-118">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="da9a5-119">Рекомендуемая задержка между GETs — 5 секунд.</span><span class="sxs-lookup"><span data-stu-id="da9a5-119">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="da9a5-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da9a5-120">Permissions</span></span>

<span data-ttu-id="da9a5-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da9a5-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da9a5-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da9a5-123">Permission type</span></span>      | <span data-ttu-id="da9a5-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da9a5-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da9a5-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da9a5-125">Delegated (work or school account)</span></span>     | <span data-ttu-id="da9a5-126">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da9a5-126">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="da9a5-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da9a5-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da9a5-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da9a5-128">Not supported.</span></span>    |
|<span data-ttu-id="da9a5-129">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da9a5-129">Application</span></span>                            | <span data-ttu-id="da9a5-130">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da9a5-130">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da9a5-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da9a5-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="da9a5-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da9a5-132">Request headers</span></span>
| <span data-ttu-id="da9a5-133">Заголовок</span><span class="sxs-lookup"><span data-stu-id="da9a5-133">Header</span></span>       | <span data-ttu-id="da9a5-134">Значение</span><span class="sxs-lookup"><span data-stu-id="da9a5-134">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="da9a5-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da9a5-135">Authorization</span></span>  | <span data-ttu-id="da9a5-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da9a5-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="da9a5-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da9a5-138">Content-Type</span></span>  | <span data-ttu-id="da9a5-139">application/json</span><span class="sxs-lookup"><span data-stu-id="da9a5-139">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="da9a5-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da9a5-140">Request body</span></span>

| <span data-ttu-id="da9a5-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="da9a5-141">Property</span></span>     | <span data-ttu-id="da9a5-142">Тип</span><span class="sxs-lookup"><span data-stu-id="da9a5-142">Type</span></span>   |<span data-ttu-id="da9a5-143">Описание</span><span class="sxs-lookup"><span data-stu-id="da9a5-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da9a5-144">classification</span><span class="sxs-lookup"><span data-stu-id="da9a5-144">classification</span></span>|<span data-ttu-id="da9a5-145">String (необязательный)</span><span class="sxs-lookup"><span data-stu-id="da9a5-145">String (optional)</span></span>|<span data-ttu-id="da9a5-146">Описывает классификацию для группы (например, низкое, среднее или высокое влияние бизнеса).</span><span class="sxs-lookup"><span data-stu-id="da9a5-146">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="da9a5-147">Допустимые значения для этого свойства определяются путем создания значения параметра [ClassificationList](../resources/directorysetting.md) на основе [определения шаблона.](../resources/directorysettingtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="da9a5-147">Valid values for this property are defined by creating a ClassificationList [setting](../resources/directorysetting.md) value, based on the [template definition](../resources/directorysettingtemplate.md).</span></span> <span data-ttu-id="da9a5-148">Если классификация не указана, классификация будет скопирована из исходной группы или группы.</span><span class="sxs-lookup"><span data-stu-id="da9a5-148">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="da9a5-149">description</span><span class="sxs-lookup"><span data-stu-id="da9a5-149">description</span></span>|<span data-ttu-id="da9a5-150">String (необязательный)</span><span class="sxs-lookup"><span data-stu-id="da9a5-150">String (optional)</span></span>|<span data-ttu-id="da9a5-151">Необязательное описание для группы.</span><span class="sxs-lookup"><span data-stu-id="da9a5-151">An optional description for the group.</span></span> <span data-ttu-id="da9a5-152">Если это свойство не указано, оно останется пустым.</span><span class="sxs-lookup"><span data-stu-id="da9a5-152">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="da9a5-153">displayName</span><span class="sxs-lookup"><span data-stu-id="da9a5-153">displayName</span></span>|<span data-ttu-id="da9a5-154">String</span><span class="sxs-lookup"><span data-stu-id="da9a5-154">String</span></span>|<span data-ttu-id="da9a5-p109">Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления. Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="da9a5-p109">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="da9a5-158">mailNickname</span><span class="sxs-lookup"><span data-stu-id="da9a5-158">mailNickname</span></span>|<span data-ttu-id="da9a5-159">String</span><span class="sxs-lookup"><span data-stu-id="da9a5-159">String</span></span>|<span data-ttu-id="da9a5-160">Почтовый псевдоним для группы (уникальный в организации).</span><span class="sxs-lookup"><span data-stu-id="da9a5-160">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="da9a5-161">Это свойство должно быть указано при создании группы.</span><span class="sxs-lookup"><span data-stu-id="da9a5-161">This property must be specified when a group is created.</span></span> <span data-ttu-id="da9a5-162">Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="da9a5-162">Supports $filter.</span></span> <span data-ttu-id="da9a5-163">Если это свойство не указано, оно будет вычисляться из displayName.</span><span class="sxs-lookup"><span data-stu-id="da9a5-163">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="da9a5-164">Известная проблема: это свойство в настоящее время игнорируется.</span><span class="sxs-lookup"><span data-stu-id="da9a5-164">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="da9a5-165">partsToClone</span><span class="sxs-lookup"><span data-stu-id="da9a5-165">partsToClone</span></span>| [<span data-ttu-id="da9a5-166">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="da9a5-166">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="da9a5-167">Разделенный запятой список частей для клонирования.</span><span class="sxs-lookup"><span data-stu-id="da9a5-167">A comma-separated list of the parts to clone.</span></span> <span data-ttu-id="da9a5-168">Юридическими частями являются "приложения, вкладки, параметры, каналы, члены".</span><span class="sxs-lookup"><span data-stu-id="da9a5-168">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="da9a5-169">visibility</span><span class="sxs-lookup"><span data-stu-id="da9a5-169">visibility</span></span>|<span data-ttu-id="da9a5-170">[teamVisibilityType](../resources/teamvisibilitytype.md) (необязательный)</span><span class="sxs-lookup"><span data-stu-id="da9a5-170">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span></span>| <span data-ttu-id="da9a5-171">Указывает видимость группы.</span><span class="sxs-lookup"><span data-stu-id="da9a5-171">Specifies the visibility of the group.</span></span> <span data-ttu-id="da9a5-172">Возможные значения: **Private**, **Public**.</span><span class="sxs-lookup"><span data-stu-id="da9a5-172">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="da9a5-173">Если видимость не указана, видимость будет скопирована из исходной группы или группы.</span><span class="sxs-lookup"><span data-stu-id="da9a5-173">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="da9a5-174">Если клонированная группа является командой **educationClass,** параметр видимости игнорируется, а видимость новой группы будет задана в hiddenMembership.</span><span class="sxs-lookup"><span data-stu-id="da9a5-174">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="da9a5-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="da9a5-175">Response</span></span>

<span data-ttu-id="da9a5-176">В случае успешного использования этот метод возвращает код ответа с заготвом `202 Accepted` Location: header, указывав на [ресурс](../resources/teamsasyncoperation.md) операции.</span><span class="sxs-lookup"><span data-stu-id="da9a5-176">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="da9a5-177">По завершению операции ресурс операции покажет вам id созданной команды.</span><span class="sxs-lookup"><span data-stu-id="da9a5-177">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="da9a5-178">Пример</span><span class="sxs-lookup"><span data-stu-id="da9a5-178">Example</span></span>
#### <a name="request"></a><span data-ttu-id="da9a5-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="da9a5-179">Request</span></span>
<span data-ttu-id="da9a5-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da9a5-180">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="da9a5-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="da9a5-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "clone_team"
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
# <a name="c"></a>[<span data-ttu-id="da9a5-182">C#</span><span class="sxs-lookup"><span data-stu-id="da9a5-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/clone-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da9a5-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da9a5-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/clone-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da9a5-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da9a5-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/clone-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da9a5-185">Java</span><span class="sxs-lookup"><span data-stu-id="da9a5-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/clone-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="da9a5-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="da9a5-186">Response</span></span>
<span data-ttu-id="da9a5-187">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="da9a5-187">The following is an example of the response.</span></span> <span data-ttu-id="da9a5-188">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="da9a5-188">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
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
  "suppressions": []
}
-->


