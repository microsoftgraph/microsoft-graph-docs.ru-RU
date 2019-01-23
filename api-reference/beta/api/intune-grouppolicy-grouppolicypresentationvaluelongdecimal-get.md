---
title: Получение groupPolicyPresentationValueLongDecimal
description: Чтение свойства и связи объекта groupPolicyPresentationValueLongDecimal.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 63ffecef20cc3760d89ac2933b1c1e32c1e60f93
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430717"
---
# <a name="get-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="4a8e2-103">Получение groupPolicyPresentationValueLongDecimal</span><span class="sxs-lookup"><span data-stu-id="4a8e2-103">Get groupPolicyPresentationValueLongDecimal</span></span>

> <span data-ttu-id="4a8e2-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4a8e2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4a8e2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a8e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a8e2-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a8e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a8e2-107">Чтение свойства и связи объекта [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="4a8e2-107">Read properties and relationships of the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a8e2-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="4a8e2-108">Prerequisites</span></span>
<span data-ttu-id="4a8e2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4a8e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4a8e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a8e2-111">Permission type</span></span>|<span data-ttu-id="4a8e2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a8e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a8e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a8e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a8e2-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a8e2-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="4a8e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a8e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a8e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a8e2-116">Not supported.</span></span>|
|<span data-ttu-id="4a8e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a8e2-117">Application</span></span>|<span data-ttu-id="4a8e2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a8e2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a8e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a8e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4a8e2-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4a8e2-120">Optional query parameters</span></span>
<span data-ttu-id="4a8e2-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4a8e2-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a8e2-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a8e2-122">Request headers</span></span>
|<span data-ttu-id="4a8e2-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a8e2-123">Header</span></span>|<span data-ttu-id="4a8e2-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4a8e2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a8e2-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a8e2-125">Authorization</span></span>|<span data-ttu-id="4a8e2-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4a8e2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a8e2-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4a8e2-127">Accept</span></span>|<span data-ttu-id="4a8e2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4a8e2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a8e2-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a8e2-129">Request body</span></span>
<span data-ttu-id="4a8e2-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a8e2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a8e2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a8e2-131">Response</span></span>
<span data-ttu-id="4a8e2-132">Успешно завершена, этот метод возвращает `200 OK` объект [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4a8e2-132">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a8e2-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4a8e2-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a8e2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a8e2-134">Request</span></span>
<span data-ttu-id="4a8e2-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a8e2-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

### <a name="response"></a><span data-ttu-id="4a8e2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a8e2-136">Response</span></span>
<span data-ttu-id="4a8e2-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4a8e2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 297

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "id": "210f7078-7078-210f-7870-0f2178700f21",
    "value": 5
  }
}
```




