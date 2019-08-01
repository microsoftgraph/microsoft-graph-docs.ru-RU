---
title: Создание telecomExpenseManagementPartner
description: Создание объекта telecomExpenseManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 58399603c12c7560dc1707b3c4badcee6700d6cb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023379"
---
# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="e1a1b-103">Создание telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="e1a1b-103">Create telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="e1a1b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e1a1b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1a1b-105">Создание объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="e1a1b-105">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1a1b-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e1a1b-106">Prerequisites</span></span>
<span data-ttu-id="e1a1b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1a1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1a1b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1a1b-109">Permission type</span></span>|<span data-ttu-id="e1a1b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1a1b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1a1b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1a1b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e1a1b-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1a1b-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e1a1b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1a1b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1a1b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1a1b-114">Not supported.</span></span>|
|<span data-ttu-id="e1a1b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1a1b-115">Application</span></span>|<span data-ttu-id="e1a1b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1a1b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1a1b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1a1b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="e1a1b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1a1b-118">Request headers</span></span>
|<span data-ttu-id="e1a1b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e1a1b-119">Header</span></span>|<span data-ttu-id="e1a1b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e1a1b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1a1b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1a1b-121">Authorization</span></span>|<span data-ttu-id="e1a1b-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1a1b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1a1b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e1a1b-123">Accept</span></span>|<span data-ttu-id="e1a1b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e1a1b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1a1b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e1a1b-125">Request body</span></span>
<span data-ttu-id="e1a1b-126">В теле запроса добавьте представление объекта telecomExpenseManagementPartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1a1b-126">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="e1a1b-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта telecomExpenseManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="e1a1b-127">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="e1a1b-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1a1b-128">Property</span></span>|<span data-ttu-id="e1a1b-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e1a1b-129">Type</span></span>|<span data-ttu-id="e1a1b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e1a1b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1a1b-131">id</span><span class="sxs-lookup"><span data-stu-id="e1a1b-131">id</span></span>|<span data-ttu-id="e1a1b-132">String</span><span class="sxs-lookup"><span data-stu-id="e1a1b-132">String</span></span>|<span data-ttu-id="e1a1b-133">Уникальный идентификатор партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="e1a1b-133">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="e1a1b-134">displayName</span><span class="sxs-lookup"><span data-stu-id="e1a1b-134">displayName</span></span>|<span data-ttu-id="e1a1b-135">Строка</span><span class="sxs-lookup"><span data-stu-id="e1a1b-135">String</span></span>|<span data-ttu-id="e1a1b-136">Отображаемое имя партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="e1a1b-136">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="e1a1b-137">url</span><span class="sxs-lookup"><span data-stu-id="e1a1b-137">url</span></span>|<span data-ttu-id="e1a1b-138">String</span><span class="sxs-lookup"><span data-stu-id="e1a1b-138">String</span></span>|<span data-ttu-id="e1a1b-139">URL-адрес административной панели управления партнера TEM, где администратор может настроить службу TEM.</span><span class="sxs-lookup"><span data-stu-id="e1a1b-139">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="e1a1b-140">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="e1a1b-140">appAuthorized</span></span>|<span data-ttu-id="e1a1b-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1a1b-141">Boolean</span></span>|<span data-ttu-id="e1a1b-142">Определяет, разрешен ли доступ к Intune партнерскому приложению AAD.</span><span class="sxs-lookup"><span data-stu-id="e1a1b-142">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="e1a1b-143">enabled</span><span class="sxs-lookup"><span data-stu-id="e1a1b-143">enabled</span></span>|<span data-ttu-id="e1a1b-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1a1b-144">Boolean</span></span>|<span data-ttu-id="e1a1b-145">Определяет, включено или отключено сейчас подключение Intune к службе TEM.</span><span class="sxs-lookup"><span data-stu-id="e1a1b-145">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="e1a1b-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="e1a1b-146">lastConnectionDateTime</span></span>|<span data-ttu-id="e1a1b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1a1b-147">DateTimeOffset</span></span>|<span data-ttu-id="e1a1b-148">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="e1a1b-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="e1a1b-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1a1b-149">Response</span></span>
<span data-ttu-id="e1a1b-150">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e1a1b-150">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1a1b-151">Пример</span><span class="sxs-lookup"><span data-stu-id="e1a1b-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1a1b-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1a1b-152">Request</span></span>
<span data-ttu-id="e1a1b-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1a1b-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners
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

### <a name="response"></a><span data-ttu-id="e1a1b-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1a1b-154">Response</span></span>
<span data-ttu-id="e1a1b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1a1b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



