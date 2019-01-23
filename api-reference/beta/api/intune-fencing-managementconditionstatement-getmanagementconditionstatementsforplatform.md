---
title: функция getManagementConditionStatementsForPlatform
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cf8e3daec196adc6b9124d91e66b82ab78a03337
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419669"
---
# <a name="getmanagementconditionstatementsforplatform-function"></a><span data-ttu-id="15979-103">функция getManagementConditionStatementsForPlatform</span><span class="sxs-lookup"><span data-stu-id="15979-103">getManagementConditionStatementsForPlatform function</span></span>

> <span data-ttu-id="15979-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="15979-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="15979-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15979-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15979-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15979-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15979-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="15979-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15979-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="15979-108">Prerequisites</span></span>
<span data-ttu-id="15979-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="15979-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="15979-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15979-111">Permission type</span></span>|<span data-ttu-id="15979-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="15979-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15979-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15979-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15979-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="15979-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="15979-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15979-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15979-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15979-116">Not supported.</span></span>|
|<span data-ttu-id="15979-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15979-117">Application</span></span>|<span data-ttu-id="15979-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15979-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15979-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15979-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/getManagementConditionStatementsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="15979-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15979-120">Request headers</span></span>
|<span data-ttu-id="15979-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15979-121">Header</span></span>|<span data-ttu-id="15979-122">Значение</span><span class="sxs-lookup"><span data-stu-id="15979-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15979-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15979-123">Authorization</span></span>|<span data-ttu-id="15979-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="15979-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15979-125">Accept</span><span class="sxs-lookup"><span data-stu-id="15979-125">Accept</span></span>|<span data-ttu-id="15979-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15979-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15979-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15979-127">Request body</span></span>
<span data-ttu-id="15979-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="15979-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="15979-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="15979-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="15979-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="15979-130">Property</span></span>|<span data-ttu-id="15979-131">Тип</span><span class="sxs-lookup"><span data-stu-id="15979-131">Type</span></span>|<span data-ttu-id="15979-132">Описание</span><span class="sxs-lookup"><span data-stu-id="15979-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15979-133">platform</span><span class="sxs-lookup"><span data-stu-id="15979-133">platform</span></span>|[<span data-ttu-id="15979-134">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="15979-134">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="15979-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="15979-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="15979-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="15979-136">Response</span></span>
<span data-ttu-id="15979-137">Если успешно завершена, эта функция возвращает `200 OK` код ответа и семейства [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="15979-137">If successful, this function returns a `200 OK` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15979-138">Пример</span><span class="sxs-lookup"><span data-stu-id="15979-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="15979-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="15979-139">Request</span></span>
<span data-ttu-id="15979-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15979-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="15979-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="15979-141">Response</span></span>
<span data-ttu-id="15979-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="15979-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managementConditionStatement",
      "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "expression": {
        "@odata.type": "microsoft.graph.managementConditionExpression"
      },
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```




