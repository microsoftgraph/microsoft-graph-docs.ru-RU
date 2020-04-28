---
title: Действие assign
description: Замените все целевые группы для политики.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 91becd14da5731d81a9c1764871fad1ef2f0ebdb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43392202"
---
# <a name="assign-action"></a><span data-ttu-id="365ed-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="365ed-103">assign action</span></span>

<span data-ttu-id="365ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="365ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="365ed-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="365ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="365ed-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="365ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="365ed-107">Замените все целевые группы для политики.</span><span class="sxs-lookup"><span data-stu-id="365ed-107">Replace all targeted groups for a policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="365ed-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="365ed-108">Prerequisites</span></span>
<span data-ttu-id="365ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="365ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="365ed-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="365ed-111">Permission type</span></span>|<span data-ttu-id="365ed-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="365ed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="365ed-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="365ed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="365ed-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="365ed-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="365ed-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="365ed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="365ed-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="365ed-116">Not supported.</span></span>|
|<span data-ttu-id="365ed-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="365ed-117">Application</span></span>|<span data-ttu-id="365ed-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="365ed-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="365ed-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="365ed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="365ed-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="365ed-120">Request headers</span></span>
|<span data-ttu-id="365ed-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="365ed-121">Header</span></span>|<span data-ttu-id="365ed-122">Значение</span><span class="sxs-lookup"><span data-stu-id="365ed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="365ed-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="365ed-123">Authorization</span></span>|<span data-ttu-id="365ed-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="365ed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="365ed-125">Accept</span><span class="sxs-lookup"><span data-stu-id="365ed-125">Accept</span></span>|<span data-ttu-id="365ed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="365ed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="365ed-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="365ed-127">Request body</span></span>
<span data-ttu-id="365ed-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="365ed-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="365ed-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="365ed-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="365ed-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="365ed-130">Property</span></span>|<span data-ttu-id="365ed-131">Тип</span><span class="sxs-lookup"><span data-stu-id="365ed-131">Type</span></span>|<span data-ttu-id="365ed-132">Описание</span><span class="sxs-lookup"><span data-stu-id="365ed-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="365ed-133">оффицеконфигуратионассигнментс</span><span class="sxs-lookup"><span data-stu-id="365ed-133">officeConfigurationAssignments</span></span>|<span data-ttu-id="365ed-134">Коллекция [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="365ed-134">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="365ed-135">Список назначений конфигурации Office</span><span class="sxs-lookup"><span data-stu-id="365ed-135">List of office configuration assignments</span></span>|



## <a name="response"></a><span data-ttu-id="365ed-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="365ed-136">Response</span></span>
<span data-ttu-id="365ed-137">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="365ed-137">If successful, this action returns a `200 OK` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="365ed-138">Пример</span><span class="sxs-lookup"><span data-stu-id="365ed-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="365ed-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="365ed-139">Request</span></span>
<span data-ttu-id="365ed-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="365ed-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="365ed-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="365ed-141">Response</span></span>
<span data-ttu-id="365ed-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="365ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



