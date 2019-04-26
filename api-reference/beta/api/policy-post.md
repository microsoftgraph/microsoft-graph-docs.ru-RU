---
title: Создание политики
description: Создайте новый объект Policy, указав отображаемое имя, тип политики и описание политики.
localization_priority: Normal
ms.openlocfilehash: 4521f6fb032f936aec27cc5cac47d27e62bd2a3a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332201"
---
# <a name="create-policy"></a><span data-ttu-id="47548-103">Создание политики</span><span class="sxs-lookup"><span data-stu-id="47548-103">Create Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47548-104">Создайте новый объект [Policy](../resources/policy.md) , указав отображаемое имя, тип политики и описание политики.</span><span class="sxs-lookup"><span data-stu-id="47548-104">Create a new [policy](../resources/policy.md) object by specifying display name, policy type, and policy description.</span></span>

><span data-ttu-id="47548-105">Note: сведения о политике будут проверены, прежде чем они будут сохранены.</span><span class="sxs-lookup"><span data-stu-id="47548-105">Note: The policy details will be validated before being stored.</span></span> <span data-ttu-id="47548-106">Если он не проходит проверку, возвращается неверный запрос 400.</span><span class="sxs-lookup"><span data-stu-id="47548-106">If it does not pass validation, a 400 Bad Request will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="47548-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47548-107">Permissions</span></span>
<span data-ttu-id="47548-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47548-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47548-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47548-110">Permission type</span></span>      | <span data-ttu-id="47548-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47548-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47548-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47548-112">Delegated (work or school account)</span></span> | <span data-ttu-id="47548-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="47548-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="47548-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47548-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47548-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47548-115">Not supported.</span></span>    |
|<span data-ttu-id="47548-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47548-116">Application</span></span> | <span data-ttu-id="47548-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47548-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="47548-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47548-118">HTTP request</span></span>

```http
POST /policies
```
## <a name="request-headers"></a><span data-ttu-id="47548-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47548-119">Request headers</span></span>
| <span data-ttu-id="47548-120">Имя</span><span class="sxs-lookup"><span data-stu-id="47548-120">Name</span></span>       | <span data-ttu-id="47548-121">Тип</span><span class="sxs-lookup"><span data-stu-id="47548-121">Type</span></span> | <span data-ttu-id="47548-122">Описание</span><span class="sxs-lookup"><span data-stu-id="47548-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="47548-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="47548-123">Authorization</span></span>  | <span data-ttu-id="47548-124">string</span><span class="sxs-lookup"><span data-stu-id="47548-124">string</span></span>  | <span data-ttu-id="47548-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47548-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="47548-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="47548-127">Content-Type</span></span> | <span data-ttu-id="47548-128">application/json</span><span class="sxs-lookup"><span data-stu-id="47548-128">application/json</span></span>  | <span data-ttu-id="47548-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47548-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47548-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47548-131">Request body</span></span>
<span data-ttu-id="47548-132">В тексте запроса предоставьте представление объекта [Policy](../resources/policy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47548-132">In the request body, provide a JSON representation of [policy](../resources/policy.md) object.</span></span>

<span data-ttu-id="47548-133">В следующей таблице приведены свойства, необходимые при создании политики.</span><span class="sxs-lookup"><span data-stu-id="47548-133">The following table shows the properties that are required when you create a policy.</span></span>

| <span data-ttu-id="47548-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="47548-134">Parameter</span></span>    | <span data-ttu-id="47548-135">Тип</span><span class="sxs-lookup"><span data-stu-id="47548-135">Type</span></span>   |<span data-ttu-id="47548-136">Описание</span><span class="sxs-lookup"><span data-stu-id="47548-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47548-137">RDLC</span><span class="sxs-lookup"><span data-stu-id="47548-137">definition</span></span>|<span data-ttu-id="47548-138">String</span><span class="sxs-lookup"><span data-stu-id="47548-138">String</span></span>|<span data-ttu-id="47548-139">Строковая версия объекта [Policy](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="47548-139">The string version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="47548-140">displayName</span><span class="sxs-lookup"><span data-stu-id="47548-140">displayName</span></span>|<span data-ttu-id="47548-141">String</span><span class="sxs-lookup"><span data-stu-id="47548-141">String</span></span>|<span data-ttu-id="47548-142">Настраиваемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="47548-142">A custom name for the policy.</span></span>|
|<span data-ttu-id="47548-143">type</span><span class="sxs-lookup"><span data-stu-id="47548-143">type</span></span>|<span data-ttu-id="47548-144">String</span><span class="sxs-lookup"><span data-stu-id="47548-144">String</span></span>|<span data-ttu-id="47548-145">Указывает тип политики.</span><span class="sxs-lookup"><span data-stu-id="47548-145">Specifies the type of policy.</span></span> <span data-ttu-id="47548-146">В настоящее время должен быть "Токенлифетимеполици"</span><span class="sxs-lookup"><span data-stu-id="47548-146">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="47548-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="47548-147">Response</span></span>

<span data-ttu-id="47548-148">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [Policy](../resources/policy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="47548-148">If successful, this method returns `201 Created` response code and [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="47548-149">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="47548-149">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>  

## <a name="example"></a><span data-ttu-id="47548-150">Пример</span><span class="sxs-lookup"><span data-stu-id="47548-150">Example</span></span>
<span data-ttu-id="47548-151">В приведенном ниже примере создается новая политика срока действия маркера.</span><span class="sxs-lookup"><span data-stu-id="47548-151">The following example creates a new token lifetime Policy.</span></span> <span data-ttu-id="47548-152">Обратите внимание, что параметр определения строки имеет экранированные двойные кавычки.</span><span class="sxs-lookup"><span data-stu-id="47548-152">Notice the string definition parameter has escaped double quotes.</span></span>

##### <a name="request"></a><span data-ttu-id="47548-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="47548-153">Request</span></span>
<span data-ttu-id="47548-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47548-154">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/policies
Content-Type: application/json

{
  "displayName":"CustomTokenLifetimePolicy",
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "type":"TokenLifetimePolicy"
}
```

##### <a name="response"></a><span data-ttu-id="47548-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="47548-155">Response</span></span>
<span data-ttu-id="47548-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47548-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
