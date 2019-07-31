---
title: Действие updatePriorities
description: Обновление приоритетов политики.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 964b8c85764193852b80edfb150be8ec6f867b2a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35958937"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="e7710-103">Действие updatePriorities</span><span class="sxs-lookup"><span data-stu-id="e7710-103">updatePriorities action</span></span>

> <span data-ttu-id="e7710-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7710-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7710-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e7710-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7710-106">Обновление приоритетов политики.</span><span class="sxs-lookup"><span data-stu-id="e7710-106">Update policy priorities.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7710-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e7710-107">Prerequisites</span></span>
<span data-ttu-id="e7710-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7710-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7710-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7710-110">Permission type</span></span>|<span data-ttu-id="e7710-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7710-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7710-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7710-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7710-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7710-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7710-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7710-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7710-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7710-115">Not supported.</span></span>|
|<span data-ttu-id="e7710-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7710-116">Application</span></span>|<span data-ttu-id="e7710-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7710-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7710-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7710-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="e7710-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7710-119">Request headers</span></span>
|<span data-ttu-id="e7710-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e7710-120">Header</span></span>|<span data-ttu-id="e7710-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e7710-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7710-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e7710-122">Authorization</span></span>|<span data-ttu-id="e7710-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7710-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7710-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e7710-124">Accept</span></span>|<span data-ttu-id="e7710-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7710-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7710-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e7710-126">Request body</span></span>
<span data-ttu-id="e7710-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7710-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e7710-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e7710-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e7710-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7710-129">Property</span></span>|<span data-ttu-id="e7710-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e7710-130">Type</span></span>|<span data-ttu-id="e7710-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e7710-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7710-132">Оффицеконфигуратионполициидс</span><span class="sxs-lookup"><span data-stu-id="e7710-132">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="e7710-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e7710-133">String collection</span></span>|<span data-ttu-id="e7710-134">Список идентификаторов политик конфигурации Office</span><span class="sxs-lookup"><span data-stu-id="e7710-134">List of office configuration policy ids</span></span>|
|<span data-ttu-id="e7710-135">Оффицеконфигуратионприоритиес</span><span class="sxs-lookup"><span data-stu-id="e7710-135">officeConfigurationPriorities</span></span>|<span data-ttu-id="e7710-136">Коллекция Int32</span><span class="sxs-lookup"><span data-stu-id="e7710-136">Int32 collection</span></span>|<span data-ttu-id="e7710-137">Список приоритетов конфигурации Office</span><span class="sxs-lookup"><span data-stu-id="e7710-137">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="e7710-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7710-138">Response</span></span>
<span data-ttu-id="e7710-139">В случае успешного выполнения это действие возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="e7710-139">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e7710-140">Пример</span><span class="sxs-lookup"><span data-stu-id="e7710-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7710-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7710-141">Request</span></span>
<span data-ttu-id="e7710-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7710-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e7710-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7710-143">Response</span></span>
<span data-ttu-id="e7710-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e7710-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```



