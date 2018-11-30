---
title: Создание политики
description: Создание нового объекта политики, указав отображаемое имя, тип политики и описание политики.
ms.openlocfilehash: fca6201d7afa6a78f15da0d37fb611e4114783e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081947"
---
# <a name="create-policy"></a><span data-ttu-id="47b45-103">Создание политики</span><span class="sxs-lookup"><span data-stu-id="47b45-103">Create Policy</span></span>

> <span data-ttu-id="47b45-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="47b45-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47b45-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47b45-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="47b45-106">Создание нового объекта [политики](../resources/policy.md) , указав отображаемое имя, тип политики и описание политики.</span><span class="sxs-lookup"><span data-stu-id="47b45-106">Create a new [policy](../resources/policy.md) object by specifying display name, policy type, and policy description.</span></span>

><span data-ttu-id="47b45-107">Примечание: Сведения о политике проверяются перед сохранением.</span><span class="sxs-lookup"><span data-stu-id="47b45-107">Note: The policy details will be validated before being stored.</span></span> <span data-ttu-id="47b45-108">Если он не пройдет проверку, 400 Неверный запрос будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="47b45-108">If it does not pass validation, a 400 Bad Request will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="47b45-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47b45-109">Permissions</span></span>
<span data-ttu-id="47b45-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47b45-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47b45-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47b45-112">Permission type</span></span>      | <span data-ttu-id="47b45-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47b45-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47b45-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47b45-114">Delegated (work or school account)</span></span> | <span data-ttu-id="47b45-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="47b45-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="47b45-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47b45-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47b45-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47b45-117">Not supported.</span></span>    |
|<span data-ttu-id="47b45-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47b45-118">Application</span></span> | <span data-ttu-id="47b45-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47b45-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="47b45-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47b45-120">HTTP request</span></span>

```http
POST /policies
```
## <a name="request-headers"></a><span data-ttu-id="47b45-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47b45-121">Request headers</span></span>
| <span data-ttu-id="47b45-122">Имя</span><span class="sxs-lookup"><span data-stu-id="47b45-122">Name</span></span>       | <span data-ttu-id="47b45-123">Тип</span><span class="sxs-lookup"><span data-stu-id="47b45-123">Type</span></span> | <span data-ttu-id="47b45-124">Описание</span><span class="sxs-lookup"><span data-stu-id="47b45-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="47b45-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="47b45-125">Authorization</span></span>  | <span data-ttu-id="47b45-126">string</span><span class="sxs-lookup"><span data-stu-id="47b45-126">string</span></span>  | <span data-ttu-id="47b45-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47b45-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="47b45-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="47b45-129">Content-Type</span></span> | <span data-ttu-id="47b45-130">application/json</span><span class="sxs-lookup"><span data-stu-id="47b45-130">application/json</span></span>  | <span data-ttu-id="47b45-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47b45-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47b45-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47b45-133">Request body</span></span>
<span data-ttu-id="47b45-134">В тексте запроса для представления JSON объекта [политики](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="47b45-134">In the request body, provide a JSON representation of [policy](../resources/policy.md) object.</span></span>

<span data-ttu-id="47b45-135">В следующей таблице приведены свойства, необходимых при создании политики.</span><span class="sxs-lookup"><span data-stu-id="47b45-135">The following table shows the properties that are required when you create a policy.</span></span>

| <span data-ttu-id="47b45-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="47b45-136">Parameter</span></span>    | <span data-ttu-id="47b45-137">Тип</span><span class="sxs-lookup"><span data-stu-id="47b45-137">Type</span></span>   |<span data-ttu-id="47b45-138">Description</span><span class="sxs-lookup"><span data-stu-id="47b45-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47b45-139">definition</span><span class="sxs-lookup"><span data-stu-id="47b45-139">definition</span></span>|<span data-ttu-id="47b45-140">String</span><span class="sxs-lookup"><span data-stu-id="47b45-140">String</span></span>|<span data-ttu-id="47b45-141">Строковая версия объекта [политики](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="47b45-141">The string version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="47b45-142">displayName</span><span class="sxs-lookup"><span data-stu-id="47b45-142">displayName</span></span>|<span data-ttu-id="47b45-143">String</span><span class="sxs-lookup"><span data-stu-id="47b45-143">String</span></span>|<span data-ttu-id="47b45-144">Пользовательское имя для политики.</span><span class="sxs-lookup"><span data-stu-id="47b45-144">A custom name for the policy.</span></span>|
|<span data-ttu-id="47b45-145">type</span><span class="sxs-lookup"><span data-stu-id="47b45-145">type</span></span>|<span data-ttu-id="47b45-146">String</span><span class="sxs-lookup"><span data-stu-id="47b45-146">String</span></span>|<span data-ttu-id="47b45-147">Указывает тип политики.</span><span class="sxs-lookup"><span data-stu-id="47b45-147">Specifies the type of policy.</span></span> <span data-ttu-id="47b45-148">В настоящее время должен быть «TokenLifetimePolicy»</span><span class="sxs-lookup"><span data-stu-id="47b45-148">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="47b45-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="47b45-149">Response</span></span>

<span data-ttu-id="47b45-150">Успешно завершена, этот метод возвращает `201 Created` ответа кода и [политики](../resources/policy.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="47b45-150">If successful, this method returns `201 Created` response code and [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="47b45-151">В случае неудачи `4xx` будут возвращены с подробные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="47b45-151">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>  

## <a name="example"></a><span data-ttu-id="47b45-152">Пример</span><span class="sxs-lookup"><span data-stu-id="47b45-152">Example</span></span>
<span data-ttu-id="47b45-153">В следующем примере создается новый срока жизни маркера политики.</span><span class="sxs-lookup"><span data-stu-id="47b45-153">The following example creates a new token lifetime Policy.</span></span> <span data-ttu-id="47b45-154">Обратите внимание на то, что параметр определения строки escape-двойные кавычки.</span><span class="sxs-lookup"><span data-stu-id="47b45-154">Notice the string definition parameter has escaped double quotes.</span></span>

##### <a name="request"></a><span data-ttu-id="47b45-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="47b45-155">Request</span></span>
<span data-ttu-id="47b45-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47b45-156">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/policies
Content-Type: application/json

{
  "displayName":"CustomTokenLifetimePolicy",
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "type":"TokenLifetimePolicy"
}
```

##### <a name="response"></a><span data-ttu-id="47b45-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="47b45-157">Response</span></span>
<span data-ttu-id="47b45-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="47b45-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
