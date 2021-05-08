---
title: 'updatableAsset: регистрацияAssets'
description: Регистрация ресурсов updatableAsset в управлении обновлениями службой развертывания.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: e83dd02ded297cde0e80b535a9d4fcb01ed45ae6
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241252"
---
# <a name="updatableasset-enrollassets"></a><span data-ttu-id="ab05e-103">updatableAsset: регистрацияAssets</span><span class="sxs-lookup"><span data-stu-id="ab05e-103">updatableAsset: enrollAssets</span></span>
<span data-ttu-id="ab05e-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="ab05e-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab05e-105">Регистрация [ресурсов updatableAsset](../resources/windowsupdates-updatableasset.md) в управлении обновлениями службой развертывания.</span><span class="sxs-lookup"><span data-stu-id="ab05e-105">Enroll [updatableAsset](../resources/windowsupdates-updatableasset.md) resources in update management by the deployment service.</span></span>

<span data-ttu-id="ab05e-106">Вы можете записать ресурс [azureADDevice](../resources/windowsupdates-azureaddevice.md) в управление обновлениями, но не зарегистрировать [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) в управлении обновлениями.</span><span class="sxs-lookup"><span data-stu-id="ab05e-106">You can enroll an [azureADDevice](../resources/windowsupdates-azureaddevice.md) resource in update management, but may not enroll an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) in update management.</span></span>

<span data-ttu-id="ab05e-107">Регистрация устройства Azure AD в управлении обновлениями автоматически создает объект **azureADDevice,** если он еще не существует.</span><span class="sxs-lookup"><span data-stu-id="ab05e-107">Enrolling an Azure AD device in update management automatically creates an **azureADDevice** object if it does not already exist.</span></span>

<span data-ttu-id="ab05e-108">Вы также можете использовать метод [enrollAssetsById](windowsupdates-updatableasset-enrollassetsbyid.md) для регистрации активов.</span><span class="sxs-lookup"><span data-stu-id="ab05e-108">You can also use the method [enrollAssetsById](windowsupdates-updatableasset-enrollassetsbyid.md) to enroll assets.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab05e-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab05e-109">Permissions</span></span>
<span data-ttu-id="ab05e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab05e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab05e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab05e-112">Permission type</span></span>|<span data-ttu-id="ab05e-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab05e-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab05e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab05e-114">Delegated (work or school account)</span></span>|<span data-ttu-id="ab05e-115">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab05e-115">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="ab05e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab05e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab05e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab05e-117">Not supported.</span></span>|
|<span data-ttu-id="ab05e-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab05e-118">Application</span></span>|<span data-ttu-id="ab05e-119">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab05e-119">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab05e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab05e-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/enrollAssets
```

## <a name="request-headers"></a><span data-ttu-id="ab05e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab05e-121">Request headers</span></span>
|<span data-ttu-id="ab05e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ab05e-122">Name</span></span>|<span data-ttu-id="ab05e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ab05e-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ab05e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab05e-124">Authorization</span></span>|<span data-ttu-id="ab05e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab05e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ab05e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab05e-127">Content-Type</span></span>|<span data-ttu-id="ab05e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab05e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab05e-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab05e-130">Request body</span></span>
<span data-ttu-id="ab05e-131">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab05e-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ab05e-132">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="ab05e-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ab05e-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="ab05e-133">Parameter</span></span>|<span data-ttu-id="ab05e-134">Тип</span><span class="sxs-lookup"><span data-stu-id="ab05e-134">Type</span></span>|<span data-ttu-id="ab05e-135">Описание</span><span class="sxs-lookup"><span data-stu-id="ab05e-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab05e-136">updateCategory</span><span class="sxs-lookup"><span data-stu-id="ab05e-136">updateCategory</span></span>|<span data-ttu-id="ab05e-137">microsoft.graph.windowsUpdates.updateCategory</span><span class="sxs-lookup"><span data-stu-id="ab05e-137">microsoft.graph.windowsUpdates.updateCategory</span></span>|<span data-ttu-id="ab05e-138">Категория обновлений для управления службой.</span><span class="sxs-lookup"><span data-stu-id="ab05e-138">The category of updates for the service to manage.</span></span> <span data-ttu-id="ab05e-139">Поддерживает подмножество значений **для updateCategory.**</span><span class="sxs-lookup"><span data-stu-id="ab05e-139">Supports a subset of the values for **updateCategory**.</span></span> <span data-ttu-id="ab05e-140">Возможные значения: `feature` .</span><span class="sxs-lookup"><span data-stu-id="ab05e-140">Possible values are: `feature`.</span></span>|
|<span data-ttu-id="ab05e-141">assets</span><span class="sxs-lookup"><span data-stu-id="ab05e-141">assets</span></span>|<span data-ttu-id="ab05e-142">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="ab05e-142">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="ab05e-143">Список **ресурсов updatableAsset** для регистрации в управлении обновлениями службой для данного **обновленияCategory.**</span><span class="sxs-lookup"><span data-stu-id="ab05e-143">List of **updatableAsset** resources to enroll in update management by the service for the given **updateCategory**.</span></span>|

## <a name="response"></a><span data-ttu-id="ab05e-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab05e-144">Response</span></span>

<span data-ttu-id="ab05e-145">В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="ab05e-145">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="ab05e-146">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ab05e-146">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ab05e-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="ab05e-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ab05e-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab05e-148">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ab05e-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab05e-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updatableasset_enrollassets"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/enrollAssets
Content-Type: application/json

{
  "updateCategory": "String",
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="ab05e-150">C#</span><span class="sxs-lookup"><span data-stu-id="ab05e-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updatableasset-enrollassets-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab05e-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab05e-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updatableasset-enrollassets-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab05e-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab05e-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updatableasset-enrollassets-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ab05e-153">Java</span><span class="sxs-lookup"><span data-stu-id="ab05e-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/updatableasset-enrollassets-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ab05e-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab05e-154">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

