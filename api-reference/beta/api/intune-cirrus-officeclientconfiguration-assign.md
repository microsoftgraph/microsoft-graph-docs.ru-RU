---
title: Действие assign
description: Замените все целевые группы для политики.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aa0ce371f61b13b5b987fc82fe5329305ec30e65
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49244579"
---
# <a name="assign-action"></a><span data-ttu-id="65f17-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="65f17-103">assign action</span></span>

<span data-ttu-id="65f17-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65f17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65f17-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65f17-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65f17-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="65f17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65f17-107">Замените все целевые группы для политики.</span><span class="sxs-lookup"><span data-stu-id="65f17-107">Replace all targeted groups for a policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65f17-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="65f17-108">Prerequisites</span></span>
<span data-ttu-id="65f17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65f17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65f17-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65f17-111">Permission type</span></span>|<span data-ttu-id="65f17-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="65f17-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65f17-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65f17-113">Delegated (work or school account)</span></span>|<span data-ttu-id="65f17-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65f17-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="65f17-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65f17-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65f17-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65f17-116">Not supported.</span></span>|
|<span data-ttu-id="65f17-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="65f17-117">Application</span></span>|<span data-ttu-id="65f17-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65f17-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65f17-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65f17-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="65f17-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="65f17-120">Request headers</span></span>
|<span data-ttu-id="65f17-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="65f17-121">Header</span></span>|<span data-ttu-id="65f17-122">Значение</span><span class="sxs-lookup"><span data-stu-id="65f17-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65f17-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65f17-123">Authorization</span></span>|<span data-ttu-id="65f17-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65f17-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65f17-125">Accept</span><span class="sxs-lookup"><span data-stu-id="65f17-125">Accept</span></span>|<span data-ttu-id="65f17-126">application/json</span><span class="sxs-lookup"><span data-stu-id="65f17-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65f17-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65f17-127">Request body</span></span>
<span data-ttu-id="65f17-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65f17-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="65f17-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="65f17-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="65f17-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="65f17-130">Property</span></span>|<span data-ttu-id="65f17-131">Тип</span><span class="sxs-lookup"><span data-stu-id="65f17-131">Type</span></span>|<span data-ttu-id="65f17-132">Описание</span><span class="sxs-lookup"><span data-stu-id="65f17-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65f17-133">оффицеконфигуратионассигнментс</span><span class="sxs-lookup"><span data-stu-id="65f17-133">officeConfigurationAssignments</span></span>|<span data-ttu-id="65f17-134">Коллекция [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="65f17-134">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="65f17-135">Список назначений конфигурации Office</span><span class="sxs-lookup"><span data-stu-id="65f17-135">List of office configuration assignments</span></span>|



## <a name="response"></a><span data-ttu-id="65f17-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="65f17-136">Response</span></span>
<span data-ttu-id="65f17-137">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="65f17-137">If successful, this action returns a `200 OK` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65f17-138">Пример</span><span class="sxs-lookup"><span data-stu-id="65f17-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="65f17-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="65f17-139">Request</span></span>
<span data-ttu-id="65f17-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65f17-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="65f17-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="65f17-141">Response</span></span>
<span data-ttu-id="65f17-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65f17-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




