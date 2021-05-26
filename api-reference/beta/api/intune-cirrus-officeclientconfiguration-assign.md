---
title: Office конфигурации клиента назначить действие
description: Замените все целевые группы для политики.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4fb8f6d2bb05e5809337ed4be0010f8f6cb470f4
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665957"
---
# <a name="office-client-configuration-assign--assign-action"></a><span data-ttu-id="5ce78-103">Office конфигурации клиента назначить действие</span><span class="sxs-lookup"><span data-stu-id="5ce78-103">Office client configuration assign  assign action</span></span>

<span data-ttu-id="5ce78-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ce78-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ce78-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ce78-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ce78-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ce78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ce78-107">Замените все целевые группы для политики.</span><span class="sxs-lookup"><span data-stu-id="5ce78-107">Replace all targeted groups for a policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ce78-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5ce78-108">Prerequisites</span></span>
<span data-ttu-id="5ce78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ce78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ce78-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ce78-111">Permission type</span></span>|<span data-ttu-id="5ce78-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ce78-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ce78-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ce78-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ce78-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ce78-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5ce78-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ce78-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ce78-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ce78-116">Not supported.</span></span>|
|<span data-ttu-id="5ce78-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5ce78-117">Application</span></span>|<span data-ttu-id="5ce78-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ce78-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ce78-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ce78-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="5ce78-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5ce78-120">Request headers</span></span>
|<span data-ttu-id="5ce78-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5ce78-121">Header</span></span>|<span data-ttu-id="5ce78-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5ce78-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ce78-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ce78-123">Authorization</span></span>|<span data-ttu-id="5ce78-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ce78-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ce78-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5ce78-125">Accept</span></span>|<span data-ttu-id="5ce78-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ce78-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ce78-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ce78-127">Request body</span></span>
<span data-ttu-id="5ce78-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ce78-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5ce78-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="5ce78-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5ce78-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ce78-130">Property</span></span>|<span data-ttu-id="5ce78-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5ce78-131">Type</span></span>|<span data-ttu-id="5ce78-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5ce78-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ce78-133">OfficeConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="5ce78-133">officeConfigurationAssignments</span></span>|<span data-ttu-id="5ce78-134">[коллекция officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5ce78-134">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="5ce78-135">Список назначений конфигурации офиса</span><span class="sxs-lookup"><span data-stu-id="5ce78-135">List of office configuration assignments</span></span>|



## <a name="response"></a><span data-ttu-id="5ce78-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ce78-136">Response</span></span>
<span data-ttu-id="5ce78-137">В случае успешного выполнения это действие возвращает код отклика и `200 OK` [коллекцию officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5ce78-137">If successful, this action returns a `200 OK` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ce78-138">Пример</span><span class="sxs-lookup"><span data-stu-id="5ce78-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ce78-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ce78-139">Request</span></span>
<span data-ttu-id="5ce78-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ce78-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5ce78-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ce78-141">Response</span></span>
<span data-ttu-id="5ce78-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5ce78-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




