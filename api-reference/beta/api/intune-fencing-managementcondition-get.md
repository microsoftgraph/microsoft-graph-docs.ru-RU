---
title: Получение managementCondition
description: Чтение свойства и связи объекта managementCondition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cf1b71e102f739188dabe04326f2c09961c88bed
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419921"
---
# <a name="get-managementcondition"></a><span data-ttu-id="42eec-103">Получение managementCondition</span><span class="sxs-lookup"><span data-stu-id="42eec-103">Get managementCondition</span></span>

> <span data-ttu-id="42eec-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="42eec-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="42eec-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42eec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42eec-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42eec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42eec-107">Чтение свойства и связи объекта [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="42eec-107">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42eec-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="42eec-108">Prerequisites</span></span>
<span data-ttu-id="42eec-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="42eec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="42eec-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42eec-111">Permission type</span></span>|<span data-ttu-id="42eec-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42eec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42eec-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42eec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42eec-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="42eec-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="42eec-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42eec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42eec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42eec-116">Not supported.</span></span>|
|<span data-ttu-id="42eec-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42eec-117">Application</span></span>|<span data-ttu-id="42eec-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42eec-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42eec-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42eec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42eec-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="42eec-120">Optional query parameters</span></span>
<span data-ttu-id="42eec-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="42eec-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42eec-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42eec-122">Request headers</span></span>
|<span data-ttu-id="42eec-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42eec-123">Header</span></span>|<span data-ttu-id="42eec-124">Значение</span><span class="sxs-lookup"><span data-stu-id="42eec-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42eec-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42eec-125">Authorization</span></span>|<span data-ttu-id="42eec-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="42eec-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42eec-127">Accept</span><span class="sxs-lookup"><span data-stu-id="42eec-127">Accept</span></span>|<span data-ttu-id="42eec-128">application/json</span><span class="sxs-lookup"><span data-stu-id="42eec-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42eec-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42eec-129">Request body</span></span>
<span data-ttu-id="42eec-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42eec-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42eec-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="42eec-131">Response</span></span>
<span data-ttu-id="42eec-132">Успешно завершена, этот метод возвращает `200 OK` объект [managementCondition](../resources/intune-fencing-managementcondition.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="42eec-132">If successful, this method returns a `200 OK` response code and [managementCondition](../resources/intune-fencing-managementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42eec-133">Пример</span><span class="sxs-lookup"><span data-stu-id="42eec-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="42eec-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="42eec-134">Request</span></span>
<span data-ttu-id="42eec-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42eec-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="42eec-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="42eec-136">Response</span></span>
<span data-ttu-id="42eec-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="42eec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 468

{
  "value": {
    "@odata.type": "#microsoft.graph.managementCondition",
    "id": "5cb49381-9381-5cb4-8193-b45c8193b45c",
    "uniqueName": "Unique Name value",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "eTag": "ETag value",
    "applicablePlatforms": [
      "androidForWork"
    ]
  }
}
```




