---
title: Список свойства carttoclassassociations
description: Список свойств и связей объектов КарттоклассассоЦиатион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 686b7f6f789bb2e2befa45976a365d979374e5df
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36340417"
---
# <a name="list-carttoclassassociations"></a><span data-ttu-id="ff063-103">Список свойства carttoclassassociations</span><span class="sxs-lookup"><span data-stu-id="ff063-103">List cartToClassAssociations</span></span>

> <span data-ttu-id="ff063-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff063-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff063-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff063-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff063-106">Список свойств и связей объектов [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="ff063-106">List properties and relationships of the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff063-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ff063-107">Prerequisites</span></span>
<span data-ttu-id="ff063-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff063-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff063-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff063-110">Permission type</span></span>|<span data-ttu-id="ff063-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff063-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff063-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff063-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ff063-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff063-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ff063-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff063-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff063-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff063-115">Not supported.</span></span>|
|<span data-ttu-id="ff063-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff063-116">Application</span></span>|<span data-ttu-id="ff063-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff063-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff063-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff063-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/cartToClassAssociations
```

## <a name="request-headers"></a><span data-ttu-id="ff063-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff063-119">Request headers</span></span>
|<span data-ttu-id="ff063-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff063-120">Header</span></span>|<span data-ttu-id="ff063-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ff063-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff063-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff063-122">Authorization</span></span>|<span data-ttu-id="ff063-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff063-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff063-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ff063-124">Accept</span></span>|<span data-ttu-id="ff063-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ff063-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff063-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ff063-126">Request body</span></span>
<span data-ttu-id="ff063-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ff063-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff063-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff063-128">Response</span></span>
<span data-ttu-id="ff063-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ff063-129">If successful, this method returns a `200 OK` response code and a collection of [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff063-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ff063-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff063-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff063-131">Request</span></span>
<span data-ttu-id="ff063-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff063-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations
```

### <a name="response"></a><span data-ttu-id="ff063-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff063-133">Response</span></span>
<span data-ttu-id="ff063-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff063-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 528

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cartToClassAssociation",
      "id": "9bdc58dd-58dd-9bdc-dd58-dc9bdd58dc9b",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "displayName": "Display Name value",
      "description": "Description value",
      "deviceCartIds": [
        "Device Cart Ids value"
      ],
      "classroomIds": [
        "Classroom Ids value"
      ]
    }
  ]
}
```






