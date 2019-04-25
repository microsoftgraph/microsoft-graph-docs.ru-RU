---
title: Функция Жетманажементкондитионстатементсфорплатформ
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e7874e0080d19b4cadb350b5198a80d1f080ed1c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532172"
---
# <a name="getmanagementconditionstatementsforplatform-function"></a><span data-ttu-id="ccad4-103">Функция Жетманажементкондитионстатементсфорплатформ</span><span class="sxs-lookup"><span data-stu-id="ccad4-103">getManagementConditionStatementsForPlatform function</span></span>

> <span data-ttu-id="ccad4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccad4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccad4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ccad4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccad4-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ccad4-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ccad4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ccad4-107">Prerequisites</span></span>
<span data-ttu-id="ccad4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccad4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccad4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccad4-110">Permission type</span></span>|<span data-ttu-id="ccad4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccad4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccad4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccad4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ccad4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccad4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ccad4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccad4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccad4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccad4-115">Not supported.</span></span>|
|<span data-ttu-id="ccad4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccad4-116">Application</span></span>|<span data-ttu-id="ccad4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccad4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccad4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccad4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/getManagementConditionStatementsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="ccad4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccad4-119">Request headers</span></span>
|<span data-ttu-id="ccad4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ccad4-120">Header</span></span>|<span data-ttu-id="ccad4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ccad4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccad4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ccad4-122">Authorization</span></span>|<span data-ttu-id="ccad4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccad4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccad4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ccad4-124">Accept</span></span>|<span data-ttu-id="ccad4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ccad4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccad4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ccad4-126">Request body</span></span>
<span data-ttu-id="ccad4-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="ccad4-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ccad4-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="ccad4-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ccad4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ccad4-129">Property</span></span>|<span data-ttu-id="ccad4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ccad4-130">Type</span></span>|<span data-ttu-id="ccad4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ccad4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccad4-132">platform</span><span class="sxs-lookup"><span data-stu-id="ccad4-132">platform</span></span>|[<span data-ttu-id="ccad4-133">Девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="ccad4-133">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="ccad4-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ccad4-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ccad4-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="ccad4-135">Response</span></span>
<span data-ttu-id="ccad4-136">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ccad4-136">If successful, this function returns a `200 OK` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccad4-137">Пример</span><span class="sxs-lookup"><span data-stu-id="ccad4-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccad4-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccad4-138">Request</span></span>
<span data-ttu-id="ccad4-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccad4-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="ccad4-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccad4-140">Response</span></span>
<span data-ttu-id="ccad4-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccad4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





