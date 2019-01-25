---
title: Создание политики
description: Создание нового объекта политики, указав отображаемое имя, тип политики и описание политики.
localization_priority: Normal
ms.openlocfilehash: 30a311b45f9705a07b62541a4f3a110daade09fa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527698"
---
# <a name="create-policy"></a><span data-ttu-id="08ece-103">Создание политики</span><span class="sxs-lookup"><span data-stu-id="08ece-103">Create Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08ece-104">Создание нового объекта [политики](../resources/policy.md) , указав отображаемое имя, тип политики и описание политики.</span><span class="sxs-lookup"><span data-stu-id="08ece-104">Create a new [policy](../resources/policy.md) object by specifying display name, policy type, and policy description.</span></span>

><span data-ttu-id="08ece-105">Примечание: Сведения о политике проверяются перед сохранением.</span><span class="sxs-lookup"><span data-stu-id="08ece-105">Note: The policy details will be validated before being stored.</span></span> <span data-ttu-id="08ece-106">Если он не пройдет проверку, 400 Неверный запрос будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="08ece-106">If it does not pass validation, a 400 Bad Request will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="08ece-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08ece-107">Permissions</span></span>
<span data-ttu-id="08ece-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08ece-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08ece-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08ece-110">Permission type</span></span>      | <span data-ttu-id="08ece-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08ece-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08ece-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08ece-112">Delegated (work or school account)</span></span> | <span data-ttu-id="08ece-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="08ece-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="08ece-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08ece-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08ece-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08ece-115">Not supported.</span></span>    |
|<span data-ttu-id="08ece-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08ece-116">Application</span></span> | <span data-ttu-id="08ece-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08ece-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08ece-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08ece-118">HTTP request</span></span>

```http
POST /policies
```
## <a name="request-headers"></a><span data-ttu-id="08ece-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08ece-119">Request headers</span></span>
| <span data-ttu-id="08ece-120">Имя</span><span class="sxs-lookup"><span data-stu-id="08ece-120">Name</span></span>       | <span data-ttu-id="08ece-121">Тип</span><span class="sxs-lookup"><span data-stu-id="08ece-121">Type</span></span> | <span data-ttu-id="08ece-122">Описание</span><span class="sxs-lookup"><span data-stu-id="08ece-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="08ece-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08ece-123">Authorization</span></span>  | <span data-ttu-id="08ece-124">string</span><span class="sxs-lookup"><span data-stu-id="08ece-124">string</span></span>  | <span data-ttu-id="08ece-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08ece-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08ece-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08ece-127">Content-Type</span></span> | <span data-ttu-id="08ece-128">application/json</span><span class="sxs-lookup"><span data-stu-id="08ece-128">application/json</span></span>  | <span data-ttu-id="08ece-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08ece-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08ece-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08ece-131">Request body</span></span>
<span data-ttu-id="08ece-132">В тексте запроса для представления JSON объекта [политики](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="08ece-132">In the request body, provide a JSON representation of [policy](../resources/policy.md) object.</span></span>

<span data-ttu-id="08ece-133">В следующей таблице приведены свойства, необходимых при создании политики.</span><span class="sxs-lookup"><span data-stu-id="08ece-133">The following table shows the properties that are required when you create a policy.</span></span>

| <span data-ttu-id="08ece-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="08ece-134">Parameter</span></span>    | <span data-ttu-id="08ece-135">Тип</span><span class="sxs-lookup"><span data-stu-id="08ece-135">Type</span></span>   |<span data-ttu-id="08ece-136">Описание</span><span class="sxs-lookup"><span data-stu-id="08ece-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08ece-137">definition</span><span class="sxs-lookup"><span data-stu-id="08ece-137">definition</span></span>|<span data-ttu-id="08ece-138">String</span><span class="sxs-lookup"><span data-stu-id="08ece-138">String</span></span>|<span data-ttu-id="08ece-139">Строковая версия объекта [политики](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="08ece-139">The string version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="08ece-140">displayName</span><span class="sxs-lookup"><span data-stu-id="08ece-140">displayName</span></span>|<span data-ttu-id="08ece-141">String</span><span class="sxs-lookup"><span data-stu-id="08ece-141">String</span></span>|<span data-ttu-id="08ece-142">Пользовательское имя для политики.</span><span class="sxs-lookup"><span data-stu-id="08ece-142">A custom name for the policy.</span></span>|
|<span data-ttu-id="08ece-143">type</span><span class="sxs-lookup"><span data-stu-id="08ece-143">type</span></span>|<span data-ttu-id="08ece-144">String</span><span class="sxs-lookup"><span data-stu-id="08ece-144">String</span></span>|<span data-ttu-id="08ece-145">Указывает тип политики.</span><span class="sxs-lookup"><span data-stu-id="08ece-145">Specifies the type of policy.</span></span> <span data-ttu-id="08ece-146">В настоящее время должен быть «TokenLifetimePolicy»</span><span class="sxs-lookup"><span data-stu-id="08ece-146">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="08ece-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="08ece-147">Response</span></span>

<span data-ttu-id="08ece-148">Успешно завершена, этот метод возвращает `201 Created` ответа кода и [политики](../resources/policy.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="08ece-148">If successful, this method returns `201 Created` response code and [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="08ece-149">В случае неудачи `4xx` будут возвращены с подробные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="08ece-149">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>  

## <a name="example"></a><span data-ttu-id="08ece-150">Пример</span><span class="sxs-lookup"><span data-stu-id="08ece-150">Example</span></span>
<span data-ttu-id="08ece-151">В следующем примере создается новый срока жизни маркера политики.</span><span class="sxs-lookup"><span data-stu-id="08ece-151">The following example creates a new token lifetime Policy.</span></span> <span data-ttu-id="08ece-152">Обратите внимание на то, что параметр определения строки escape-двойные кавычки.</span><span class="sxs-lookup"><span data-stu-id="08ece-152">Notice the string definition parameter has escaped double quotes.</span></span>

##### <a name="request"></a><span data-ttu-id="08ece-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="08ece-153">Request</span></span>
<span data-ttu-id="08ece-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08ece-154">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/policies
Content-Type: application/json

{
  "displayName":"CustomTokenLifetimePolicy",
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "type":"TokenLifetimePolicy"
}
```

##### <a name="response"></a><span data-ttu-id="08ece-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="08ece-155">Response</span></span>
<span data-ttu-id="08ece-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="08ece-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#policies/$entity",
  "id":"id-value",
  "alternativeIdentifier":null,
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "displayName":"name-value",
  "isOrganizationDefault":false,
  "keyCredentials",
  "type":"TokenLifetimePolicy"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
