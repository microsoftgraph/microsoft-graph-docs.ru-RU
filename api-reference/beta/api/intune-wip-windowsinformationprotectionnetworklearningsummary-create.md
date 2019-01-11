---
title: Создание объекта windowsInformationProtectionNetworkLearningSummary
description: Создание объекта windowsInformationProtectionNetworkLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f3cb295fd24b70b4d40464218532fd1298fd2ab1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841505"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="ad9d4-103">Создание объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="ad9d4-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="ad9d4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ad9d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad9d4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad9d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad9d4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ad9d4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad9d4-107">Создание объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="ad9d4-107">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad9d4-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ad9d4-108">Prerequisites</span></span>
<span data-ttu-id="ad9d4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad9d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad9d4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad9d4-111">Permission type</span></span>|<span data-ttu-id="ad9d4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad9d4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad9d4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad9d4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad9d4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad9d4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ad9d4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad9d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad9d4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad9d4-116">Not supported.</span></span>|
|<span data-ttu-id="ad9d4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad9d4-117">Application</span></span>|<span data-ttu-id="ad9d4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad9d4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad9d4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad9d4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="ad9d4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad9d4-120">Request headers</span></span>
|<span data-ttu-id="ad9d4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad9d4-121">Header</span></span>|<span data-ttu-id="ad9d4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ad9d4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad9d4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad9d4-123">Authorization</span></span>|<span data-ttu-id="ad9d4-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ad9d4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad9d4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ad9d4-125">Accept</span></span>|<span data-ttu-id="ad9d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad9d4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad9d4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ad9d4-127">Request body</span></span>
<span data-ttu-id="ad9d4-128">В теле запроса добавьте представление объекта windowsInformationProtectionNetworkLearningSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad9d4-128">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="ad9d4-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="ad9d4-129">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="ad9d4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad9d4-130">Property</span></span>|<span data-ttu-id="ad9d4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ad9d4-131">Type</span></span>|<span data-ttu-id="ad9d4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ad9d4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad9d4-133">id</span><span class="sxs-lookup"><span data-stu-id="ad9d4-133">id</span></span>|<span data-ttu-id="ad9d4-134">String</span><span class="sxs-lookup"><span data-stu-id="ad9d4-134">String</span></span>|<span data-ttu-id="ad9d4-135">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="ad9d4-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="ad9d4-136">url</span><span class="sxs-lookup"><span data-stu-id="ad9d4-136">url</span></span>|<span data-ttu-id="ad9d4-137">String</span><span class="sxs-lookup"><span data-stu-id="ad9d4-137">String</span></span>|<span data-ttu-id="ad9d4-138">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="ad9d4-138">Website url</span></span>|
|<span data-ttu-id="ad9d4-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="ad9d4-139">deviceCount</span></span>|<span data-ttu-id="ad9d4-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ad9d4-140">Int32</span></span>|<span data-ttu-id="ad9d4-141">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="ad9d4-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="ad9d4-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad9d4-142">Response</span></span>
<span data-ttu-id="ad9d4-143">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ad9d4-143">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad9d4-144">Пример</span><span class="sxs-lookup"><span data-stu-id="ad9d4-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad9d4-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad9d4-145">Request</span></span>
<span data-ttu-id="ad9d4-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad9d4-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="ad9d4-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad9d4-147">Response</span></span>
<span data-ttu-id="ad9d4-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ad9d4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```





