---
title: Действие updatePriorities
description: Обновление приоритетов политики.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6422cd3f40270f6502a58551e6c5c1b739219e00
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32483168"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="3e639-103">Действие updatePriorities</span><span class="sxs-lookup"><span data-stu-id="3e639-103">updatePriorities action</span></span>

> <span data-ttu-id="3e639-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e639-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e639-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e639-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e639-106">Обновление приоритетов политики.</span><span class="sxs-lookup"><span data-stu-id="3e639-106">Update policy priorities.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e639-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3e639-107">Prerequisites</span></span>
<span data-ttu-id="3e639-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e639-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e639-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e639-110">Permission type</span></span>|<span data-ttu-id="3e639-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e639-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e639-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e639-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3e639-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e639-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3e639-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e639-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e639-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e639-115">Not supported.</span></span>|
|<span data-ttu-id="3e639-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e639-116">Application</span></span>|<span data-ttu-id="3e639-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e639-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e639-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e639-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="3e639-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e639-119">Request headers</span></span>
|<span data-ttu-id="3e639-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e639-120">Header</span></span>|<span data-ttu-id="3e639-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3e639-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e639-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e639-122">Authorization</span></span>|<span data-ttu-id="3e639-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e639-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e639-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3e639-124">Accept</span></span>|<span data-ttu-id="3e639-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3e639-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e639-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e639-126">Request body</span></span>
<span data-ttu-id="3e639-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e639-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3e639-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="3e639-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3e639-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e639-129">Property</span></span>|<span data-ttu-id="3e639-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3e639-130">Type</span></span>|<span data-ttu-id="3e639-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3e639-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e639-132">Оффицеконфигуратионполициидс</span><span class="sxs-lookup"><span data-stu-id="3e639-132">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="3e639-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3e639-133">String collection</span></span>|<span data-ttu-id="3e639-134">Список идентификаторов политик конфигурации Office</span><span class="sxs-lookup"><span data-stu-id="3e639-134">List of office configuration policy ids</span></span>|
|<span data-ttu-id="3e639-135">Оффицеконфигуратионприоритиес</span><span class="sxs-lookup"><span data-stu-id="3e639-135">officeConfigurationPriorities</span></span>|<span data-ttu-id="3e639-136">Коллекция Int32</span><span class="sxs-lookup"><span data-stu-id="3e639-136">Int32 collection</span></span>|<span data-ttu-id="3e639-137">Список приоритетов конфигурации Office</span><span class="sxs-lookup"><span data-stu-id="3e639-137">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="3e639-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e639-138">Response</span></span>
<span data-ttu-id="3e639-139">В случае успешного выполнения это действие возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="3e639-139">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3e639-140">Пример</span><span class="sxs-lookup"><span data-stu-id="3e639-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e639-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e639-141">Request</span></span>
<span data-ttu-id="3e639-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e639-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3e639-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e639-143">Response</span></span>
<span data-ttu-id="3e639-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e639-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```



