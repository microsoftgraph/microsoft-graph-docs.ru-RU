---
title: Обновление объекта telecomExpenseManagementPartner
description: Обновление свойств объекта telecomExpenseManagementPartner.
ms.openlocfilehash: 600ceb9fc5f7ec00659438516772d37867a8a207
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024825"
---
# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="e7b6c-103">Обновление объекта telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="e7b6c-103">Update telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="e7b6c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e7b6c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7b6c-105">Обновление свойств объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="e7b6c-105">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e7b6c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e7b6c-106">Prerequisites</span></span>
<span data-ttu-id="e7b6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7b6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7b6c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7b6c-109">Permission type</span></span>|<span data-ttu-id="e7b6c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7b6c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7b6c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7b6c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e7b6c-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7b6c-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e7b6c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7b6c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7b6c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7b6c-114">Not supported.</span></span>|
|<span data-ttu-id="e7b6c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7b6c-115">Application</span></span>|<span data-ttu-id="e7b6c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7b6c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7b6c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7b6c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="e7b6c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7b6c-118">Request headers</span></span>
|<span data-ttu-id="e7b6c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e7b6c-119">Header</span></span>|<span data-ttu-id="e7b6c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e7b6c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7b6c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7b6c-121">Authorization</span></span>|<span data-ttu-id="e7b6c-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e7b6c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7b6c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e7b6c-123">Accept</span></span>|<span data-ttu-id="e7b6c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e7b6c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7b6c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e7b6c-125">Request body</span></span>
<span data-ttu-id="e7b6c-126">В теле запроса добавьте представление объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7b6c-126">In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="e7b6c-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="e7b6c-127">The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>

|<span data-ttu-id="e7b6c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7b6c-128">Property</span></span>|<span data-ttu-id="e7b6c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e7b6c-129">Type</span></span>|<span data-ttu-id="e7b6c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e7b6c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7b6c-131">id</span><span class="sxs-lookup"><span data-stu-id="e7b6c-131">id</span></span>|<span data-ttu-id="e7b6c-132">String</span><span class="sxs-lookup"><span data-stu-id="e7b6c-132">String</span></span>|<span data-ttu-id="e7b6c-133">Уникальный идентификатор партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="e7b6c-133">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="e7b6c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="e7b6c-134">displayName</span></span>|<span data-ttu-id="e7b6c-135">String</span><span class="sxs-lookup"><span data-stu-id="e7b6c-135">String</span></span>|<span data-ttu-id="e7b6c-136">Отображаемое имя партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="e7b6c-136">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="e7b6c-137">url</span><span class="sxs-lookup"><span data-stu-id="e7b6c-137">url</span></span>|<span data-ttu-id="e7b6c-138">String</span><span class="sxs-lookup"><span data-stu-id="e7b6c-138">String</span></span>|<span data-ttu-id="e7b6c-139">URL-адрес административной панели управления партнера TEM, где администратор может настроить службу TEM.</span><span class="sxs-lookup"><span data-stu-id="e7b6c-139">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="e7b6c-140">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="e7b6c-140">appAuthorized</span></span>|<span data-ttu-id="e7b6c-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7b6c-141">Boolean</span></span>|<span data-ttu-id="e7b6c-142">Определяет, разрешен ли доступ к Intune партнерскому приложению AAD.</span><span class="sxs-lookup"><span data-stu-id="e7b6c-142">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="e7b6c-143">enabled</span><span class="sxs-lookup"><span data-stu-id="e7b6c-143">enabled</span></span>|<span data-ttu-id="e7b6c-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7b6c-144">Boolean</span></span>|<span data-ttu-id="e7b6c-145">Определяет, включено или отключено сейчас подключение Intune к службе TEM.</span><span class="sxs-lookup"><span data-stu-id="e7b6c-145">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="e7b6c-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="e7b6c-146">lastConnectionDateTime</span></span>|<span data-ttu-id="e7b6c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7b6c-147">DateTimeOffset</span></span>|<span data-ttu-id="e7b6c-148">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="e7b6c-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="e7b6c-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7b6c-149">Response</span></span>
<span data-ttu-id="e7b6c-150">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e7b6c-150">If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7b6c-151">Пример</span><span class="sxs-lookup"><span data-stu-id="e7b6c-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7b6c-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7b6c-152">Request</span></span>
<span data-ttu-id="e7b6c-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7b6c-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
Content-type: application/json
Content-length: 248

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="e7b6c-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7b6c-154">Response</span></span>
<span data-ttu-id="e7b6c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e7b6c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 297

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```



