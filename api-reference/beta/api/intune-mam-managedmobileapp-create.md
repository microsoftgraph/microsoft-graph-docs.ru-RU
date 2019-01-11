---
title: Создание объекта managedMobileApp
description: Создание объекта managedMobileApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e94b95e4dfea69aafdd426fd4c9a5deca676ce42
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881104"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="7f790-103">Создание объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="7f790-103">Create managedMobileApp</span></span>

> <span data-ttu-id="7f790-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7f790-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f790-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f790-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f790-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7f790-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f790-107">Создание объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f790-107">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f790-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7f790-108">Prerequisites</span></span>
<span data-ttu-id="7f790-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f790-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f790-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f790-111">Permission type</span></span>|<span data-ttu-id="7f790-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f790-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f790-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f790-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f790-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f790-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7f790-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f790-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f790-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f790-116">Not supported.</span></span>|
|<span data-ttu-id="7f790-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f790-117">Application</span></span>|<span data-ttu-id="7f790-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f790-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f790-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f790-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
POST /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps
POST /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps
```

## <a name="request-headers"></a><span data-ttu-id="7f790-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f790-120">Request headers</span></span>
|<span data-ttu-id="7f790-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f790-121">Header</span></span>|<span data-ttu-id="7f790-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7f790-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f790-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f790-123">Authorization</span></span>|<span data-ttu-id="7f790-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7f790-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f790-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7f790-125">Accept</span></span>|<span data-ttu-id="7f790-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f790-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f790-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7f790-127">Request body</span></span>
<span data-ttu-id="7f790-128">В теле запроса добавьте представление объекта managedMobileApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f790-128">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="7f790-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="7f790-129">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="7f790-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f790-130">Property</span></span>|<span data-ttu-id="7f790-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7f790-131">Type</span></span>|<span data-ttu-id="7f790-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7f790-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f790-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="7f790-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="7f790-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="7f790-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="7f790-135">Идентификатор приложения с типом его операционной системы.</span><span class="sxs-lookup"><span data-stu-id="7f790-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="7f790-136">id</span><span class="sxs-lookup"><span data-stu-id="7f790-136">id</span></span>|<span data-ttu-id="7f790-137">Строка</span><span class="sxs-lookup"><span data-stu-id="7f790-137">String</span></span>|<span data-ttu-id="7f790-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7f790-138">Key of the entity.</span></span>|
|<span data-ttu-id="7f790-139">version</span><span class="sxs-lookup"><span data-stu-id="7f790-139">version</span></span>|<span data-ttu-id="7f790-140">Строка</span><span class="sxs-lookup"><span data-stu-id="7f790-140">String</span></span>|<span data-ttu-id="7f790-141">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="7f790-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="7f790-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f790-142">Response</span></span>
<span data-ttu-id="7f790-143">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7f790-143">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f790-144">Пример</span><span class="sxs-lookup"><span data-stu-id="7f790-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f790-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f790-145">Request</span></span>
<span data-ttu-id="7f790-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f790-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="7f790-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f790-147">Response</span></span>
<span data-ttu-id="7f790-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7f790-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 230

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "0a129715-9715-0a12-1597-120a1597120a",
  "version": "Version value"
}
```





