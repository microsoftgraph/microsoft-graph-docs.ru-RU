---
title: 'Синхронизация: Аккуиреакцесстокен'
description: Получение маркера доступа OAuth для авторизации службы подготовки Azure AD для подготовки пользователей в приложении
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fed4999b86a790389d96e26e630b270ac1b35f2d
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643762"
---
# <a name="acquireaccesstoken"></a><span data-ttu-id="c7f00-103">аккуиреакцесстокен</span><span class="sxs-lookup"><span data-stu-id="c7f00-103">acquireAccessToken</span></span>
<span data-ttu-id="c7f00-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7f00-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c7f00-105">Получите маркер доступа OAuth, чтобы авторизовать службу подготовки Azure AD для подготовки пользователей в приложении.</span><span class="sxs-lookup"><span data-stu-id="c7f00-105">Acquire an OAuth Access token to authorize the Azure AD provisioning service to provision users into an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7f00-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7f00-106">Permissions</span></span>
<span data-ttu-id="c7f00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7f00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7f00-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7f00-109">Permission type</span></span>|<span data-ttu-id="c7f00-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7f00-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7f00-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7f00-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c7f00-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7f00-112">Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="c7f00-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7f00-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7f00-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7f00-114">Not supported.</span></span>|
|<span data-ttu-id="c7f00-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7f00-115">Application</span></span>|<span data-ttu-id="c7f00-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7f00-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7f00-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7f00-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /applications/{applicationsId}/synchronization/acquireAccessToken
POST /servicePrincipals/{servicePrincipalsId}/synchronization/acquireAccessToken
```

## <a name="request-headers"></a><span data-ttu-id="c7f00-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7f00-118">Request headers</span></span>
|<span data-ttu-id="c7f00-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c7f00-119">Name</span></span>|<span data-ttu-id="c7f00-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c7f00-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c7f00-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7f00-121">Authorization</span></span>|<span data-ttu-id="c7f00-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7f00-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c7f00-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7f00-124">Content-Type</span></span>|<span data-ttu-id="c7f00-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7f00-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7f00-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7f00-127">Request body</span></span>
<span data-ttu-id="c7f00-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7f00-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c7f00-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c7f00-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c7f00-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="c7f00-130">Parameter</span></span>|<span data-ttu-id="c7f00-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c7f00-131">Type</span></span>|<span data-ttu-id="c7f00-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c7f00-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7f00-133">записей</span><span class="sxs-lookup"><span data-stu-id="c7f00-133">credentials</span></span>|<span data-ttu-id="c7f00-134">Коллекция [синчронизатионсекреткэйстрингвалуепаир](../resources/synchronization-secretkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c7f00-134">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="c7f00-135">Представляет одно секретное значение.</span><span class="sxs-lookup"><span data-stu-id="c7f00-135">Represents a single secret value.</span></span>|



## <a name="response"></a><span data-ttu-id="c7f00-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7f00-136">Response</span></span>

<span data-ttu-id="c7f00-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c7f00-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c7f00-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="c7f00-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c7f00-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7f00-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c7f00-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7f00-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronization_acquireaccesstoken"
}
-->
``` http
POST https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/acquireAccessToken
Content-Type: application/json
Content-length: 123

{
  "credentials": [
    {
      "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="c7f00-141">C#</span><span class="sxs-lookup"><span data-stu-id="c7f00-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronization-acquireaccesstoken-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7f00-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7f00-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronization-acquireaccesstoken-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7f00-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7f00-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronization-acquireaccesstoken-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c7f00-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7f00-144">Response</span></span>
<span data-ttu-id="c7f00-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c7f00-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
