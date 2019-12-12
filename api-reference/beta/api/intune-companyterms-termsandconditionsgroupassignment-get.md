---
title: Получение Термсандкондитионсграупассигнмент
description: Чтение свойств и связей объекта Термсандкондитионсграупассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 907f5ba5a29010f1c17cb95531d287bd992ad34d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955058"
---
# <a name="get-termsandconditionsgroupassignment"></a><span data-ttu-id="3a099-103">Получение Термсандкондитионсграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="3a099-103">Get termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="3a099-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a099-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a099-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a099-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a099-106">Чтение свойств и связей объекта [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="3a099-106">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a099-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3a099-107">Prerequisites</span></span>
<span data-ttu-id="3a099-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a099-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a099-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a099-110">Permission type</span></span>|<span data-ttu-id="3a099-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a099-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a099-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a099-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3a099-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a099-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3a099-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a099-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a099-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a099-115">Not supported.</span></span>|
|<span data-ttu-id="3a099-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a099-116">Application</span></span>|<span data-ttu-id="3a099-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a099-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a099-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a099-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3a099-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3a099-119">Optional query parameters</span></span>
<span data-ttu-id="3a099-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3a099-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a099-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a099-121">Request headers</span></span>
|<span data-ttu-id="3a099-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a099-122">Header</span></span>|<span data-ttu-id="3a099-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3a099-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a099-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a099-124">Authorization</span></span>|<span data-ttu-id="3a099-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a099-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a099-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3a099-126">Accept</span></span>|<span data-ttu-id="3a099-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3a099-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a099-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3a099-128">Request body</span></span>
<span data-ttu-id="3a099-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a099-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a099-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a099-130">Response</span></span>
<span data-ttu-id="3a099-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [термсандкондитионсграупассигнмент](../resources/intune-companyterms-termsandconditionsgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3a099-131">If successful, this method returns a `200 OK` response code and [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a099-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3a099-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a099-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a099-133">Request</span></span>
<span data-ttu-id="3a099-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a099-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="3a099-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a099-135">Response</span></span>
<span data-ttu-id="3a099-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a099-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 194

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
    "id": "2eb1aab7-aab7-2eb1-b7aa-b12eb7aab12e",
    "targetGroupId": "Target Group Id value"
  }
}
```





