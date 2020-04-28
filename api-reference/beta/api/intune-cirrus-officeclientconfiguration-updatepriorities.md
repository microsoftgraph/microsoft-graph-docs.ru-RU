---
title: Действие updatePriorities
description: Обновление приоритетов политики.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 07bbff5017523849d3be81b800bb2ea37eab1cd8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43392062"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="b86d1-103">Действие updatePriorities</span><span class="sxs-lookup"><span data-stu-id="b86d1-103">updatePriorities action</span></span>

<span data-ttu-id="b86d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b86d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b86d1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b86d1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b86d1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b86d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b86d1-107">Обновление приоритетов политики.</span><span class="sxs-lookup"><span data-stu-id="b86d1-107">Update policy priorities.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b86d1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b86d1-108">Prerequisites</span></span>
<span data-ttu-id="b86d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b86d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b86d1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b86d1-111">Permission type</span></span>|<span data-ttu-id="b86d1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b86d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b86d1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b86d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b86d1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b86d1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b86d1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b86d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b86d1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b86d1-116">Not supported.</span></span>|
|<span data-ttu-id="b86d1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b86d1-117">Application</span></span>|<span data-ttu-id="b86d1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b86d1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b86d1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b86d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="b86d1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b86d1-120">Request headers</span></span>
|<span data-ttu-id="b86d1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b86d1-121">Header</span></span>|<span data-ttu-id="b86d1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b86d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b86d1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b86d1-123">Authorization</span></span>|<span data-ttu-id="b86d1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b86d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b86d1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b86d1-125">Accept</span></span>|<span data-ttu-id="b86d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b86d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b86d1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b86d1-127">Request body</span></span>
<span data-ttu-id="b86d1-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b86d1-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b86d1-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="b86d1-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b86d1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b86d1-130">Property</span></span>|<span data-ttu-id="b86d1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b86d1-131">Type</span></span>|<span data-ttu-id="b86d1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b86d1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b86d1-133">оффицеконфигуратионполициидс</span><span class="sxs-lookup"><span data-stu-id="b86d1-133">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="b86d1-134">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="b86d1-134">String collection</span></span>|<span data-ttu-id="b86d1-135">Список идентификаторов политик конфигурации Office</span><span class="sxs-lookup"><span data-stu-id="b86d1-135">List of office configuration policy ids</span></span>|
|<span data-ttu-id="b86d1-136">оффицеконфигуратионприоритиес</span><span class="sxs-lookup"><span data-stu-id="b86d1-136">officeConfigurationPriorities</span></span>|<span data-ttu-id="b86d1-137">Коллекция Int32</span><span class="sxs-lookup"><span data-stu-id="b86d1-137">Int32 collection</span></span>|<span data-ttu-id="b86d1-138">Список приоритетов конфигурации Office</span><span class="sxs-lookup"><span data-stu-id="b86d1-138">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="b86d1-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="b86d1-139">Response</span></span>
<span data-ttu-id="b86d1-140">В случае успешного выполнения это действие возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="b86d1-140">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b86d1-141">Пример</span><span class="sxs-lookup"><span data-stu-id="b86d1-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="b86d1-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="b86d1-142">Request</span></span>
<span data-ttu-id="b86d1-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b86d1-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities

Content-type: application/json
Content-length: 143

{
  "officeConfigurationPolicyIds": [
    "Office Configuration Policy Ids value"
  ],
  "officeConfigurationPriorities": [
    13
  ]
}
```

### <a name="response"></a><span data-ttu-id="b86d1-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="b86d1-144">Response</span></span>
<span data-ttu-id="b86d1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b86d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```



