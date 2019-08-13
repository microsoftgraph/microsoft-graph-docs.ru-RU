---
title: Действие assign
description: Замените все целевые группы для политики.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d9d548e4ac1ec6f72b600c4e91ecd50e5e455159
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36322263"
---
# <a name="assign-action"></a><span data-ttu-id="cb8ee-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="cb8ee-103">assign action</span></span>

> <span data-ttu-id="cb8ee-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb8ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb8ee-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb8ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb8ee-106">Замените все целевые группы для политики.</span><span class="sxs-lookup"><span data-stu-id="cb8ee-106">Replace all targeted groups for a policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb8ee-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cb8ee-107">Prerequisites</span></span>
<span data-ttu-id="cb8ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb8ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb8ee-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb8ee-110">Permission type</span></span>|<span data-ttu-id="cb8ee-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb8ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb8ee-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb8ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cb8ee-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb8ee-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cb8ee-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb8ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb8ee-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb8ee-115">Not supported.</span></span>|
|<span data-ttu-id="cb8ee-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb8ee-116">Application</span></span>|<span data-ttu-id="cb8ee-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb8ee-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb8ee-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb8ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="cb8ee-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb8ee-119">Request headers</span></span>
|<span data-ttu-id="cb8ee-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb8ee-120">Header</span></span>|<span data-ttu-id="cb8ee-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cb8ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb8ee-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb8ee-122">Authorization</span></span>|<span data-ttu-id="cb8ee-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb8ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb8ee-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cb8ee-124">Accept</span></span>|<span data-ttu-id="cb8ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cb8ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb8ee-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cb8ee-126">Request body</span></span>
<span data-ttu-id="cb8ee-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb8ee-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="cb8ee-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="cb8ee-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="cb8ee-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb8ee-129">Property</span></span>|<span data-ttu-id="cb8ee-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cb8ee-130">Type</span></span>|<span data-ttu-id="cb8ee-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cb8ee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb8ee-132">оффицеконфигуратионассигнментс</span><span class="sxs-lookup"><span data-stu-id="cb8ee-132">officeConfigurationAssignments</span></span>|<span data-ttu-id="cb8ee-133">Коллекция [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cb8ee-133">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="cb8ee-134">Список назначений конфигурации Office</span><span class="sxs-lookup"><span data-stu-id="cb8ee-134">List of office configuration assignments</span></span>|



## <a name="response"></a><span data-ttu-id="cb8ee-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb8ee-135">Response</span></span>
<span data-ttu-id="cb8ee-136">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cb8ee-136">If successful, this action returns a `200 OK` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb8ee-137">Пример</span><span class="sxs-lookup"><span data-stu-id="cb8ee-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb8ee-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb8ee-138">Request</span></span>
<span data-ttu-id="cb8ee-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb8ee-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign

Content-type: application/json
Content-length: 299

{
  "officeConfigurationAssignments": [
    {
      "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
      "id": "804730f3-30f3-8047-f330-4780f3304780",
      "target": {
        "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="cb8ee-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb8ee-140">Response</span></span>
<span data-ttu-id="cb8ee-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cb8ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
      "id": "804730f3-30f3-8047-f330-4780f3304780",
      "target": {
        "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
      }
    }
  ]
}
```






