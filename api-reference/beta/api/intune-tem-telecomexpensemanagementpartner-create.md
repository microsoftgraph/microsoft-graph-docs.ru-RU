---
title: Создание telecomExpenseManagementPartner
description: Создание объекта telecomExpenseManagementPartner.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 05b7f9a2ff8eeb99c973e874ab3f085ad91a5bb7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350533"
---
# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="465ab-103">Создание telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="465ab-103">Create telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="465ab-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="465ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="465ab-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="465ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="465ab-106">Создание объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="465ab-106">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="465ab-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="465ab-107">Prerequisites</span></span>
<span data-ttu-id="465ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="465ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="465ab-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="465ab-110">Permission type</span></span>|<span data-ttu-id="465ab-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="465ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="465ab-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="465ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="465ab-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="465ab-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="465ab-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="465ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="465ab-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="465ab-115">Not supported.</span></span>|
|<span data-ttu-id="465ab-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="465ab-116">Application</span></span>|<span data-ttu-id="465ab-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="465ab-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="465ab-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="465ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="465ab-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="465ab-119">Request headers</span></span>
|<span data-ttu-id="465ab-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="465ab-120">Header</span></span>|<span data-ttu-id="465ab-121">Значение</span><span class="sxs-lookup"><span data-stu-id="465ab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="465ab-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="465ab-122">Authorization</span></span>|<span data-ttu-id="465ab-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="465ab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="465ab-124">Accept</span><span class="sxs-lookup"><span data-stu-id="465ab-124">Accept</span></span>|<span data-ttu-id="465ab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="465ab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="465ab-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="465ab-126">Request body</span></span>
<span data-ttu-id="465ab-127">В теле запроса добавьте представление объекта telecomExpenseManagementPartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="465ab-127">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="465ab-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта telecomExpenseManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="465ab-128">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="465ab-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="465ab-129">Property</span></span>|<span data-ttu-id="465ab-130">Тип</span><span class="sxs-lookup"><span data-stu-id="465ab-130">Type</span></span>|<span data-ttu-id="465ab-131">Описание</span><span class="sxs-lookup"><span data-stu-id="465ab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="465ab-132">id</span><span class="sxs-lookup"><span data-stu-id="465ab-132">id</span></span>|<span data-ttu-id="465ab-133">String</span><span class="sxs-lookup"><span data-stu-id="465ab-133">String</span></span>|<span data-ttu-id="465ab-134">Уникальный идентификатор партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="465ab-134">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="465ab-135">displayName</span><span class="sxs-lookup"><span data-stu-id="465ab-135">displayName</span></span>|<span data-ttu-id="465ab-136">Строка</span><span class="sxs-lookup"><span data-stu-id="465ab-136">String</span></span>|<span data-ttu-id="465ab-137">Отображаемое имя партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="465ab-137">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="465ab-138">url</span><span class="sxs-lookup"><span data-stu-id="465ab-138">url</span></span>|<span data-ttu-id="465ab-139">String</span><span class="sxs-lookup"><span data-stu-id="465ab-139">String</span></span>|<span data-ttu-id="465ab-140">URL-адрес административной панели управления партнера TEM, где администратор может настроить службу TEM.</span><span class="sxs-lookup"><span data-stu-id="465ab-140">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="465ab-141">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="465ab-141">appAuthorized</span></span>|<span data-ttu-id="465ab-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="465ab-142">Boolean</span></span>|<span data-ttu-id="465ab-143">Определяет, разрешен ли доступ к Intune партнерскому приложению AAD.</span><span class="sxs-lookup"><span data-stu-id="465ab-143">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="465ab-144">enabled</span><span class="sxs-lookup"><span data-stu-id="465ab-144">enabled</span></span>|<span data-ttu-id="465ab-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="465ab-145">Boolean</span></span>|<span data-ttu-id="465ab-146">Определяет, включено или отключено сейчас подключение Intune к службе TEM.</span><span class="sxs-lookup"><span data-stu-id="465ab-146">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="465ab-147">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="465ab-147">lastConnectionDateTime</span></span>|<span data-ttu-id="465ab-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="465ab-148">DateTimeOffset</span></span>|<span data-ttu-id="465ab-149">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="465ab-149">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="465ab-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="465ab-150">Response</span></span>
<span data-ttu-id="465ab-151">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="465ab-151">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="465ab-152">Пример</span><span class="sxs-lookup"><span data-stu-id="465ab-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="465ab-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="465ab-153">Request</span></span>
<span data-ttu-id="465ab-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="465ab-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners
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

### <a name="response"></a><span data-ttu-id="465ab-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="465ab-155">Response</span></span>
<span data-ttu-id="465ab-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="465ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






