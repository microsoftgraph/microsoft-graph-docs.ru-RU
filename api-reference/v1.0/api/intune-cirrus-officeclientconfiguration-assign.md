---
title: Действие assign
description: Замените все целевые группы для политики.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aa0ce371f61b13b5b987fc82fe5329305ec30e65
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754396"
---
# <a name="assign-action"></a><span data-ttu-id="b5e6a-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="b5e6a-103">assign action</span></span>

<span data-ttu-id="b5e6a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5e6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5e6a-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5e6a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5e6a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b5e6a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5e6a-107">Замените все целевые группы для политики.</span><span class="sxs-lookup"><span data-stu-id="b5e6a-107">Replace all targeted groups for a policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5e6a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b5e6a-108">Prerequisites</span></span>
<span data-ttu-id="b5e6a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5e6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5e6a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5e6a-111">Permission type</span></span>|<span data-ttu-id="b5e6a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5e6a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5e6a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5e6a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5e6a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5e6a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b5e6a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5e6a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5e6a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5e6a-116">Not supported.</span></span>|
|<span data-ttu-id="b5e6a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b5e6a-117">Application</span></span>|<span data-ttu-id="b5e6a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5e6a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5e6a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5e6a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="b5e6a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b5e6a-120">Request headers</span></span>
|<span data-ttu-id="b5e6a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b5e6a-121">Header</span></span>|<span data-ttu-id="b5e6a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b5e6a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5e6a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5e6a-123">Authorization</span></span>|<span data-ttu-id="b5e6a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5e6a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5e6a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b5e6a-125">Accept</span></span>|<span data-ttu-id="b5e6a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b5e6a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5e6a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5e6a-127">Request body</span></span>
<span data-ttu-id="b5e6a-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5e6a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b5e6a-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="b5e6a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b5e6a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5e6a-130">Property</span></span>|<span data-ttu-id="b5e6a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b5e6a-131">Type</span></span>|<span data-ttu-id="b5e6a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b5e6a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5e6a-133">OfficeConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="b5e6a-133">officeConfigurationAssignments</span></span>|<span data-ttu-id="b5e6a-134">[коллекция officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b5e6a-134">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b5e6a-135">Список назначений конфигурации офиса</span><span class="sxs-lookup"><span data-stu-id="b5e6a-135">List of office configuration assignments</span></span>|



## <a name="response"></a><span data-ttu-id="b5e6a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5e6a-136">Response</span></span>
<span data-ttu-id="b5e6a-137">В случае успешного выполнения это действие возвращает код отклика и `200 OK` [коллекцию officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b5e6a-137">If successful, this action returns a `200 OK` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5e6a-138">Пример</span><span class="sxs-lookup"><span data-stu-id="b5e6a-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5e6a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5e6a-139">Request</span></span>
<span data-ttu-id="b5e6a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5e6a-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b5e6a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5e6a-141">Response</span></span>
<span data-ttu-id="b5e6a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5e6a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




