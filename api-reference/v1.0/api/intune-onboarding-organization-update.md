---
title: Обновление организации
description: Обновление свойств объекта organization.
author: tfitzmac
ms.openlocfilehash: d26d11bb2f67b933ba5d78e444ae8e52d32339ce
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358900"
---
# <a name="update-organization"></a><span data-ttu-id="e31c7-103">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="e31c7-103">Update organization</span></span>

> <span data-ttu-id="e31c7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e31c7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e31c7-105">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="e31c7-105">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e31c7-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e31c7-106">Prerequisites</span></span>
<span data-ttu-id="e31c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e31c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e31c7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e31c7-109">Permission type</span></span>|<span data-ttu-id="e31c7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e31c7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e31c7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e31c7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e31c7-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e31c7-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e31c7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e31c7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e31c7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e31c7-114">Not supported.</span></span>|
|<span data-ttu-id="e31c7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e31c7-115">Application</span></span>|<span data-ttu-id="e31c7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e31c7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e31c7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e31c7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="e31c7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e31c7-118">Request headers</span></span>
|<span data-ttu-id="e31c7-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e31c7-119">Header</span></span>|<span data-ttu-id="e31c7-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e31c7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e31c7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e31c7-121">Authorization</span></span>|<span data-ttu-id="e31c7-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e31c7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e31c7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e31c7-123">Accept</span></span>|<span data-ttu-id="e31c7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e31c7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e31c7-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e31c7-125">Request body</span></span>
<span data-ttu-id="e31c7-126">В теле запроса добавьте представление объекта [organization](../resources/intune-onboarding-organization.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e31c7-126">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="e31c7-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="e31c7-127">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="e31c7-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e31c7-128">Property</span></span>|<span data-ttu-id="e31c7-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e31c7-129">Type</span></span>|<span data-ttu-id="e31c7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e31c7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e31c7-131">id</span><span class="sxs-lookup"><span data-stu-id="e31c7-131">id</span></span>|<span data-ttu-id="e31c7-132">Строка</span><span class="sxs-lookup"><span data-stu-id="e31c7-132">String</span></span>|<span data-ttu-id="e31c7-133">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="e31c7-133">The GUID for the object.</span></span>|
|<span data-ttu-id="e31c7-134">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="e31c7-134">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="e31c7-135">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="e31c7-135">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="e31c7-136">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="e31c7-136">Mobile device management authority.</span></span> <span data-ttu-id="e31c7-137">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="e31c7-137">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|



## <a name="response"></a><span data-ttu-id="e31c7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e31c7-138">Response</span></span>
<span data-ttu-id="e31c7-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [organization](../resources/intune-onboarding-organization.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e31c7-139">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e31c7-140">Пример</span><span class="sxs-lookup"><span data-stu-id="e31c7-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="e31c7-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="e31c7-141">Request</span></span>
<span data-ttu-id="e31c7-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e31c7-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.organization",
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="e31c7-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="e31c7-143">Response</span></span>
<span data-ttu-id="e31c7-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e31c7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 151

{
  "@odata.type": "#microsoft.graph.organization",
  "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
  "mobileDeviceManagementAuthority": "intune"
}
```



