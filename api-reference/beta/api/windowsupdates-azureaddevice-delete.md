---
title: Удаление azureADDevice
description: Удаление объекта azureADDevice.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 6cb9d23b01241878eff96e7301f8322baa7f0fb0
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068046"
---
# <a name="delete-azureaddevice"></a><span data-ttu-id="82ebe-103">Удаление azureADDevice</span><span class="sxs-lookup"><span data-stu-id="82ebe-103">Delete azureADDevice</span></span>
<span data-ttu-id="82ebe-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="82ebe-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82ebe-105">Удаление [объекта azureADDevice.](../resources/windowsupdates-azureaddevice.md)</span><span class="sxs-lookup"><span data-stu-id="82ebe-105">Delete an [azureADDevice](../resources/windowsupdates-azureaddevice.md) object.</span></span>

<span data-ttu-id="82ebe-106">При удалении устройства Azure AD оно не зарегистрируется из службы развертывания и автоматически отключается от управления службой для всех категорий обновлений, а также удаляется из каждого [развертыванияAudience](../resources/windowsupdates-deploymentaudience.md) и [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span><span class="sxs-lookup"><span data-stu-id="82ebe-106">When an Azure AD device is deleted, it is unregistered from the deployment service and automatically unenrolled from management by the service for all update categories, as well as removed from every [deploymentAudience](../resources/windowsupdates-deploymentaudience.md) and [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="82ebe-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82ebe-107">Permissions</span></span>
<span data-ttu-id="82ebe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82ebe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82ebe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82ebe-110">Permission type</span></span>|<span data-ttu-id="82ebe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82ebe-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82ebe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82ebe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82ebe-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82ebe-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="82ebe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82ebe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82ebe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82ebe-115">Not supported.</span></span>|
|<span data-ttu-id="82ebe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82ebe-116">Application</span></span>|<span data-ttu-id="82ebe-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82ebe-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82ebe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82ebe-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /admin/windows/updates/updatableAssets/{azureADDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="82ebe-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82ebe-119">Request headers</span></span>
|<span data-ttu-id="82ebe-120">Имя</span><span class="sxs-lookup"><span data-stu-id="82ebe-120">Name</span></span>|<span data-ttu-id="82ebe-121">Описание</span><span class="sxs-lookup"><span data-stu-id="82ebe-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="82ebe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82ebe-122">Authorization</span></span>|<span data-ttu-id="82ebe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82ebe-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="82ebe-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82ebe-125">Request body</span></span>
<span data-ttu-id="82ebe-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82ebe-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82ebe-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="82ebe-127">Response</span></span>

<span data-ttu-id="82ebe-p103">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="82ebe-p103">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="82ebe-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="82ebe-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="82ebe-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="82ebe-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_azureaddevice"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{azureADDeviceId}
```

### <a name="response"></a><span data-ttu-id="82ebe-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="82ebe-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

