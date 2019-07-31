---
title: Действие assign
description: Замените все целевые группы для политики.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: af53b8c39a84bfdcdd0115ac8db90bef6359303f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35958979"
---
# <a name="assign-action"></a><span data-ttu-id="7130e-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="7130e-103">assign action</span></span>

> <span data-ttu-id="7130e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7130e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7130e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7130e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7130e-106">Замените все целевые группы для политики.</span><span class="sxs-lookup"><span data-stu-id="7130e-106">Replace all targeted groups for a policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7130e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7130e-107">Prerequisites</span></span>
<span data-ttu-id="7130e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7130e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7130e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7130e-110">Permission type</span></span>|<span data-ttu-id="7130e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7130e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7130e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7130e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7130e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7130e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7130e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7130e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7130e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7130e-115">Not supported.</span></span>|
|<span data-ttu-id="7130e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7130e-116">Application</span></span>|<span data-ttu-id="7130e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7130e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7130e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7130e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="7130e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7130e-119">Request headers</span></span>
|<span data-ttu-id="7130e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7130e-120">Header</span></span>|<span data-ttu-id="7130e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7130e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7130e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7130e-122">Authorization</span></span>|<span data-ttu-id="7130e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7130e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7130e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7130e-124">Accept</span></span>|<span data-ttu-id="7130e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7130e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7130e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7130e-126">Request body</span></span>
<span data-ttu-id="7130e-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7130e-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7130e-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="7130e-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7130e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7130e-129">Property</span></span>|<span data-ttu-id="7130e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7130e-130">Type</span></span>|<span data-ttu-id="7130e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7130e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7130e-132">Оффицеконфигуратионассигнментс</span><span class="sxs-lookup"><span data-stu-id="7130e-132">officeConfigurationAssignments</span></span>|<span data-ttu-id="7130e-133">Коллекция [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7130e-133">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="7130e-134">Список назначений конфигурации Office</span><span class="sxs-lookup"><span data-stu-id="7130e-134">List of office configuration assignments</span></span>|



## <a name="response"></a><span data-ttu-id="7130e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7130e-135">Response</span></span>
<span data-ttu-id="7130e-136">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7130e-136">If successful, this action returns a `200 OK` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7130e-137">Пример</span><span class="sxs-lookup"><span data-stu-id="7130e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="7130e-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="7130e-138">Request</span></span>
<span data-ttu-id="7130e-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7130e-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7130e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="7130e-140">Response</span></span>
<span data-ttu-id="7130e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7130e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



