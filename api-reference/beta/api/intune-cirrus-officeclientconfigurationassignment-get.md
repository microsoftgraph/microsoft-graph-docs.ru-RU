---
title: Получение Оффицеклиентконфигуратионассигнмент
description: Чтение свойств и связей объекта Оффицеклиентконфигуратионассигнмент.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 22c3853d87c12af7a05c7d5808326b781be938a8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48714964"
---
# <a name="get-officeclientconfigurationassignment"></a><span data-ttu-id="bcf70-103">Получение Оффицеклиентконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="bcf70-103">Get officeClientConfigurationAssignment</span></span>

<span data-ttu-id="bcf70-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcf70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bcf70-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcf70-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcf70-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bcf70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcf70-107">Чтение свойств и связей объекта [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="bcf70-107">Read properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bcf70-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bcf70-108">Prerequisites</span></span>
<span data-ttu-id="bcf70-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcf70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcf70-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcf70-111">Permission type</span></span>|<span data-ttu-id="bcf70-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcf70-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcf70-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcf70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bcf70-114">\* \* TODO: определение областей \* \*</span><span class="sxs-lookup"><span data-stu-id="bcf70-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="bcf70-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcf70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcf70-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcf70-116">Not supported.</span></span>|
|<span data-ttu-id="bcf70-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcf70-117">Application</span></span>|<span data-ttu-id="bcf70-118">\* \* TODO: определение областей \* \*</span><span class="sxs-lookup"><span data-stu-id="bcf70-118">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcf70-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcf70-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bcf70-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bcf70-120">Optional query parameters</span></span>
<span data-ttu-id="bcf70-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bcf70-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bcf70-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcf70-122">Request headers</span></span>
|<span data-ttu-id="bcf70-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bcf70-123">Header</span></span>|<span data-ttu-id="bcf70-124">Значение</span><span class="sxs-lookup"><span data-stu-id="bcf70-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcf70-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bcf70-125">Authorization</span></span>|<span data-ttu-id="bcf70-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcf70-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcf70-127">Accept</span><span class="sxs-lookup"><span data-stu-id="bcf70-127">Accept</span></span>|<span data-ttu-id="bcf70-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bcf70-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcf70-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bcf70-129">Request body</span></span>
<span data-ttu-id="bcf70-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bcf70-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcf70-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="bcf70-131">Response</span></span>
<span data-ttu-id="bcf70-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bcf70-132">If successful, this method returns a `200 OK` response code and [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcf70-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bcf70-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="bcf70-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcf70-134">Request</span></span>
<span data-ttu-id="bcf70-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcf70-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="bcf70-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcf70-136">Response</span></span>
<span data-ttu-id="bcf70-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bcf70-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 250

{
  "value": {
    "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
    "id": "804730f3-30f3-8047-f330-4780f3304780",
    "target": {
      "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
    }
  }
}
```





