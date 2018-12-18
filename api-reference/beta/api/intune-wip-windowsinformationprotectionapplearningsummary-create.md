---
title: Создание объекта windowsInformationProtectionAppLearningSummary
description: Создание объекта windowsInformationProtectionAppLearningSummary.
author: tfitzmac
ms.openlocfilehash: 018d31a7ea356478bff2d416e13d2924931cc7cb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318755"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="e7a85-103">Создание объекта windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="e7a85-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="e7a85-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e7a85-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7a85-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7a85-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7a85-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e7a85-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7a85-107">Создание объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="e7a85-107">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e7a85-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e7a85-108">Prerequisites</span></span>
<span data-ttu-id="e7a85-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7a85-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7a85-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7a85-111">Permission type</span></span>|<span data-ttu-id="e7a85-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7a85-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7a85-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7a85-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7a85-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7a85-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e7a85-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7a85-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7a85-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7a85-116">Not supported.</span></span>|
|<span data-ttu-id="e7a85-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7a85-117">Application</span></span>|<span data-ttu-id="e7a85-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7a85-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7a85-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7a85-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="e7a85-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7a85-120">Request headers</span></span>
|<span data-ttu-id="e7a85-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e7a85-121">Header</span></span>|<span data-ttu-id="e7a85-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e7a85-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7a85-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e7a85-123">Authorization</span></span>|<span data-ttu-id="e7a85-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e7a85-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7a85-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e7a85-125">Accept</span></span>|<span data-ttu-id="e7a85-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7a85-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7a85-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e7a85-127">Request body</span></span>
<span data-ttu-id="e7a85-128">В теле запроса укажите представление объекта windowsInformationProtectionAppLearningSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7a85-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="e7a85-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="e7a85-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="e7a85-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7a85-130">Property</span></span>|<span data-ttu-id="e7a85-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e7a85-131">Type</span></span>|<span data-ttu-id="e7a85-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e7a85-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7a85-133">id</span><span class="sxs-lookup"><span data-stu-id="e7a85-133">id</span></span>|<span data-ttu-id="e7a85-134">String</span><span class="sxs-lookup"><span data-stu-id="e7a85-134">String</span></span>|<span data-ttu-id="e7a85-135">Уникальный идентификатор объекта WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="e7a85-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="e7a85-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="e7a85-136">applicationName</span></span>|<span data-ttu-id="e7a85-137">String</span><span class="sxs-lookup"><span data-stu-id="e7a85-137">String</span></span>|<span data-ttu-id="e7a85-138">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="e7a85-138">Application Name</span></span>|
|<span data-ttu-id="e7a85-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="e7a85-139">applicationType</span></span>|[<span data-ttu-id="e7a85-140">applicationType</span><span class="sxs-lookup"><span data-stu-id="e7a85-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="e7a85-141">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="e7a85-141">Application Type.</span></span> <span data-ttu-id="e7a85-142">Возможные значения: `universal`, `desktop`.</span><span class="sxs-lookup"><span data-stu-id="e7a85-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="e7a85-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="e7a85-143">deviceCount</span></span>|<span data-ttu-id="e7a85-144">Int32</span><span class="sxs-lookup"><span data-stu-id="e7a85-144">Int32</span></span>|<span data-ttu-id="e7a85-145">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="e7a85-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="e7a85-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7a85-146">Response</span></span>
<span data-ttu-id="e7a85-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e7a85-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7a85-148">Пример</span><span class="sxs-lookup"><span data-stu-id="e7a85-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7a85-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7a85-149">Request</span></span>
<span data-ttu-id="e7a85-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7a85-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="e7a85-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7a85-151">Response</span></span>
<span data-ttu-id="e7a85-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e7a85-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "063baf50-af50-063b-50af-3b0650af3b06",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```





