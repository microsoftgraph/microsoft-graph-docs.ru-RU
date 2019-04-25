---
title: Обновление объекта telecomExpenseManagementPartner
description: Обновление свойств объекта telecomExpenseManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1ca6b2dd0d55c1dc00395bdab44becb238c13f67
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576579"
---
# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="12a06-103">Обновление объекта telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="12a06-103">Update telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="12a06-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12a06-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12a06-105">Обновление свойств объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="12a06-105">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12a06-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="12a06-106">Prerequisites</span></span>
<span data-ttu-id="12a06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12a06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12a06-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12a06-109">Permission type</span></span>|<span data-ttu-id="12a06-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12a06-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12a06-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12a06-111">Delegated (work or school account)</span></span>|<span data-ttu-id="12a06-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12a06-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="12a06-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12a06-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12a06-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12a06-114">Not supported.</span></span>|
|<span data-ttu-id="12a06-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12a06-115">Application</span></span>|<span data-ttu-id="12a06-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12a06-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12a06-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12a06-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="12a06-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12a06-118">Request headers</span></span>
|<span data-ttu-id="12a06-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12a06-119">Header</span></span>|<span data-ttu-id="12a06-120">Значение</span><span class="sxs-lookup"><span data-stu-id="12a06-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12a06-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12a06-121">Authorization</span></span>|<span data-ttu-id="12a06-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12a06-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12a06-123">Accept</span><span class="sxs-lookup"><span data-stu-id="12a06-123">Accept</span></span>|<span data-ttu-id="12a06-124">application/json</span><span class="sxs-lookup"><span data-stu-id="12a06-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12a06-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12a06-125">Request body</span></span>
<span data-ttu-id="12a06-126">В теле запроса добавьте представление объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12a06-126">In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="12a06-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="12a06-127">The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>

|<span data-ttu-id="12a06-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="12a06-128">Property</span></span>|<span data-ttu-id="12a06-129">Тип</span><span class="sxs-lookup"><span data-stu-id="12a06-129">Type</span></span>|<span data-ttu-id="12a06-130">Описание</span><span class="sxs-lookup"><span data-stu-id="12a06-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12a06-131">id</span><span class="sxs-lookup"><span data-stu-id="12a06-131">id</span></span>|<span data-ttu-id="12a06-132">String</span><span class="sxs-lookup"><span data-stu-id="12a06-132">String</span></span>|<span data-ttu-id="12a06-133">Уникальный идентификатор партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="12a06-133">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="12a06-134">displayName</span><span class="sxs-lookup"><span data-stu-id="12a06-134">displayName</span></span>|<span data-ttu-id="12a06-135">Строка</span><span class="sxs-lookup"><span data-stu-id="12a06-135">String</span></span>|<span data-ttu-id="12a06-136">Отображаемое имя партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="12a06-136">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="12a06-137">url</span><span class="sxs-lookup"><span data-stu-id="12a06-137">url</span></span>|<span data-ttu-id="12a06-138">String</span><span class="sxs-lookup"><span data-stu-id="12a06-138">String</span></span>|<span data-ttu-id="12a06-139">URL-адрес административной панели управления партнера TEM, где администратор может настроить службу TEM.</span><span class="sxs-lookup"><span data-stu-id="12a06-139">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="12a06-140">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="12a06-140">appAuthorized</span></span>|<span data-ttu-id="12a06-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="12a06-141">Boolean</span></span>|<span data-ttu-id="12a06-142">Определяет, разрешен ли доступ к Intune партнерскому приложению AAD.</span><span class="sxs-lookup"><span data-stu-id="12a06-142">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="12a06-143">enabled</span><span class="sxs-lookup"><span data-stu-id="12a06-143">enabled</span></span>|<span data-ttu-id="12a06-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="12a06-144">Boolean</span></span>|<span data-ttu-id="12a06-145">Определяет, включено или отключено сейчас подключение Intune к службе TEM.</span><span class="sxs-lookup"><span data-stu-id="12a06-145">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="12a06-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="12a06-146">lastConnectionDateTime</span></span>|<span data-ttu-id="12a06-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12a06-147">DateTimeOffset</span></span>|<span data-ttu-id="12a06-148">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="12a06-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="12a06-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="12a06-149">Response</span></span>
<span data-ttu-id="12a06-150">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="12a06-150">If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12a06-151">Пример</span><span class="sxs-lookup"><span data-stu-id="12a06-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="12a06-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="12a06-152">Request</span></span>
<span data-ttu-id="12a06-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12a06-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="12a06-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="12a06-154">Response</span></span>
<span data-ttu-id="12a06-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12a06-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



