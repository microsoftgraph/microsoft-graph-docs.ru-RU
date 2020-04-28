---
title: Создание политики
description: Создайте новый объект Policy, указав отображаемое имя, тип политики и описание политики.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: dkershaw10
ms.openlocfilehash: 04bc6134529b4d7192ed50a849fc487970f6b812
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43408311"
---
# <a name="create-policy"></a><span data-ttu-id="4c8cc-103">Создание политики</span><span class="sxs-lookup"><span data-stu-id="4c8cc-103">Create Policy</span></span>

<span data-ttu-id="4c8cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c8cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c8cc-105">Создайте новый объект [Policy](../resources/policy.md) , указав отображаемое имя, тип политики и описание политики.</span><span class="sxs-lookup"><span data-stu-id="4c8cc-105">Create a new [policy](../resources/policy.md) object by specifying display name, policy type, and policy description.</span></span>

><span data-ttu-id="4c8cc-106">Note: сведения о политике будут проверены, прежде чем они будут сохранены.</span><span class="sxs-lookup"><span data-stu-id="4c8cc-106">Note: The policy details will be validated before being stored.</span></span> <span data-ttu-id="4c8cc-107">Если он не проходит проверку, возвращается неверный запрос 400.</span><span class="sxs-lookup"><span data-stu-id="4c8cc-107">If it does not pass validation, a 400 Bad Request will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c8cc-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c8cc-108">Permissions</span></span>
<span data-ttu-id="4c8cc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c8cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c8cc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c8cc-111">Permission type</span></span>      | <span data-ttu-id="4c8cc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c8cc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c8cc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c8cc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4c8cc-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4c8cc-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4c8cc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c8cc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c8cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c8cc-116">Not supported.</span></span>    |
|<span data-ttu-id="4c8cc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c8cc-117">Application</span></span> | <span data-ttu-id="4c8cc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c8cc-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c8cc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c8cc-119">HTTP request</span></span>

```http
POST /policies
```
## <a name="request-headers"></a><span data-ttu-id="4c8cc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c8cc-120">Request headers</span></span>
| <span data-ttu-id="4c8cc-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4c8cc-121">Name</span></span>       | <span data-ttu-id="4c8cc-122">Тип</span><span class="sxs-lookup"><span data-stu-id="4c8cc-122">Type</span></span> | <span data-ttu-id="4c8cc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4c8cc-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4c8cc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c8cc-124">Authorization</span></span>  | <span data-ttu-id="4c8cc-125">string</span><span class="sxs-lookup"><span data-stu-id="4c8cc-125">string</span></span>  | <span data-ttu-id="4c8cc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c8cc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4c8cc-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c8cc-128">Content-Type</span></span> | <span data-ttu-id="4c8cc-129">application/json</span><span class="sxs-lookup"><span data-stu-id="4c8cc-129">application/json</span></span>  | <span data-ttu-id="4c8cc-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c8cc-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c8cc-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c8cc-132">Request body</span></span>
<span data-ttu-id="4c8cc-133">В тексте запроса предоставьте представление объекта [Policy](../resources/policy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c8cc-133">In the request body, provide a JSON representation of [policy](../resources/policy.md) object.</span></span>

<span data-ttu-id="4c8cc-134">В следующей таблице приведены свойства, необходимые при создании политики.</span><span class="sxs-lookup"><span data-stu-id="4c8cc-134">The following table shows the properties that are required when you create a policy.</span></span>

| <span data-ttu-id="4c8cc-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="4c8cc-135">Parameter</span></span>    | <span data-ttu-id="4c8cc-136">Тип</span><span class="sxs-lookup"><span data-stu-id="4c8cc-136">Type</span></span>   |<span data-ttu-id="4c8cc-137">Описание</span><span class="sxs-lookup"><span data-stu-id="4c8cc-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c8cc-138">RDLC</span><span class="sxs-lookup"><span data-stu-id="4c8cc-138">definition</span></span>|<span data-ttu-id="4c8cc-139">String</span><span class="sxs-lookup"><span data-stu-id="4c8cc-139">String</span></span>|<span data-ttu-id="4c8cc-140">Строковая версия объекта [Policy](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="4c8cc-140">The string version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="4c8cc-141">displayName</span><span class="sxs-lookup"><span data-stu-id="4c8cc-141">displayName</span></span>|<span data-ttu-id="4c8cc-142">Строка</span><span class="sxs-lookup"><span data-stu-id="4c8cc-142">String</span></span>|<span data-ttu-id="4c8cc-143">Настраиваемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="4c8cc-143">A custom name for the policy.</span></span>|
|<span data-ttu-id="4c8cc-144">type</span><span class="sxs-lookup"><span data-stu-id="4c8cc-144">type</span></span>|<span data-ttu-id="4c8cc-145">String</span><span class="sxs-lookup"><span data-stu-id="4c8cc-145">String</span></span>|<span data-ttu-id="4c8cc-146">Указывает тип политики.</span><span class="sxs-lookup"><span data-stu-id="4c8cc-146">Specifies the type of policy.</span></span> <span data-ttu-id="4c8cc-147">В настоящее время должен быть "Токенлифетимеполици"</span><span class="sxs-lookup"><span data-stu-id="4c8cc-147">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="4c8cc-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c8cc-148">Response</span></span>

<span data-ttu-id="4c8cc-149">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [Policy](../resources/policy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c8cc-149">If successful, this method returns `201 Created` response code and [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="4c8cc-150">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="4c8cc-150">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>  

## <a name="example"></a><span data-ttu-id="4c8cc-151">Пример</span><span class="sxs-lookup"><span data-stu-id="4c8cc-151">Example</span></span>
<span data-ttu-id="4c8cc-152">В приведенном ниже примере создается новая политика срока действия маркера.</span><span class="sxs-lookup"><span data-stu-id="4c8cc-152">The following example creates a new token lifetime Policy.</span></span> <span data-ttu-id="4c8cc-153">Обратите внимание, что параметр определения строки имеет экранированные двойные кавычки.</span><span class="sxs-lookup"><span data-stu-id="4c8cc-153">Notice the string definition parameter has escaped double quotes.</span></span>

##### <a name="request"></a><span data-ttu-id="4c8cc-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c8cc-154">Request</span></span>
<span data-ttu-id="4c8cc-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c8cc-155">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/policies
Content-Type: application/json

{
  "displayName":"CustomTokenLifetimePolicy",
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "type":"TokenLifetimePolicy"
}
```

##### <a name="response"></a><span data-ttu-id="4c8cc-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c8cc-156">Response</span></span>
<span data-ttu-id="4c8cc-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c8cc-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->
