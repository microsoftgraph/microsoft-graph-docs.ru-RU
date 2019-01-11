---
title: Действие updatePriorities
description: Обновление политики приоритетов.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2aeffb76268266f239413437369cefddadb72cab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853160"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="e7d9e-103">Действие updatePriorities</span><span class="sxs-lookup"><span data-stu-id="e7d9e-103">updatePriorities action</span></span>

> <span data-ttu-id="e7d9e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e7d9e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7d9e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7d9e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7d9e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e7d9e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7d9e-107">Обновление политики приоритетов.</span><span class="sxs-lookup"><span data-stu-id="e7d9e-107">Update policy priorities.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e7d9e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e7d9e-108">Prerequisites</span></span>
<span data-ttu-id="e7d9e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7d9e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7d9e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7d9e-111">Permission type</span></span>|<span data-ttu-id="e7d9e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7d9e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7d9e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7d9e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7d9e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7d9e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7d9e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7d9e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7d9e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7d9e-116">Not supported.</span></span>|
|<span data-ttu-id="e7d9e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7d9e-117">Application</span></span>|<span data-ttu-id="e7d9e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7d9e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7d9e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7d9e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="e7d9e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7d9e-120">Request headers</span></span>
|<span data-ttu-id="e7d9e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e7d9e-121">Header</span></span>|<span data-ttu-id="e7d9e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e7d9e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7d9e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7d9e-123">Authorization</span></span>|<span data-ttu-id="e7d9e-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e7d9e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7d9e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e7d9e-125">Accept</span></span>|<span data-ttu-id="e7d9e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7d9e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7d9e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e7d9e-127">Request body</span></span>
<span data-ttu-id="e7d9e-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7d9e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e7d9e-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e7d9e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e7d9e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7d9e-130">Property</span></span>|<span data-ttu-id="e7d9e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e7d9e-131">Type</span></span>|<span data-ttu-id="e7d9e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e7d9e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7d9e-133">officeConfigurationPolicyIds</span><span class="sxs-lookup"><span data-stu-id="e7d9e-133">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="e7d9e-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e7d9e-134">String collection</span></span>|<span data-ttu-id="e7d9e-135">Список идентификаторов политики настройки office</span><span class="sxs-lookup"><span data-stu-id="e7d9e-135">List of office configuration policy ids</span></span>|
|<span data-ttu-id="e7d9e-136">officeConfigurationPriorities</span><span class="sxs-lookup"><span data-stu-id="e7d9e-136">officeConfigurationPriorities</span></span>|<span data-ttu-id="e7d9e-137">Коллекция Int32</span><span class="sxs-lookup"><span data-stu-id="e7d9e-137">Int32 collection</span></span>|<span data-ttu-id="e7d9e-138">Список приоритетов настройки office</span><span class="sxs-lookup"><span data-stu-id="e7d9e-138">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="e7d9e-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7d9e-139">Response</span></span>
<span data-ttu-id="e7d9e-140">В случае успешного выполнения это действие возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="e7d9e-140">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e7d9e-141">Пример</span><span class="sxs-lookup"><span data-stu-id="e7d9e-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7d9e-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7d9e-142">Request</span></span>
<span data-ttu-id="e7d9e-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7d9e-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e7d9e-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7d9e-144">Response</span></span>
<span data-ttu-id="e7d9e-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e7d9e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```



