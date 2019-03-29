---
title: Создание telecomExpenseManagementPartner
description: Создание объекта telecomExpenseManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 262df87456cfbea20409d4ff41566b18d896431e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970046"
---
# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="01d58-103">Создание telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="01d58-103">Create telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="01d58-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01d58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01d58-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01d58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01d58-106">Создание объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="01d58-106">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01d58-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="01d58-107">Prerequisites</span></span>
<span data-ttu-id="01d58-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01d58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01d58-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01d58-110">Permission type</span></span>|<span data-ttu-id="01d58-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01d58-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01d58-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01d58-112">Delegated (work or school account)</span></span>|<span data-ttu-id="01d58-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01d58-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="01d58-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01d58-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01d58-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01d58-115">Not supported.</span></span>|
|<span data-ttu-id="01d58-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01d58-116">Application</span></span>|<span data-ttu-id="01d58-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01d58-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01d58-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01d58-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="01d58-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01d58-119">Request headers</span></span>
|<span data-ttu-id="01d58-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01d58-120">Header</span></span>|<span data-ttu-id="01d58-121">Значение</span><span class="sxs-lookup"><span data-stu-id="01d58-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01d58-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01d58-122">Authorization</span></span>|<span data-ttu-id="01d58-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01d58-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01d58-124">Accept</span><span class="sxs-lookup"><span data-stu-id="01d58-124">Accept</span></span>|<span data-ttu-id="01d58-125">application/json</span><span class="sxs-lookup"><span data-stu-id="01d58-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01d58-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01d58-126">Request body</span></span>
<span data-ttu-id="01d58-127">В теле запроса добавьте представление объекта telecomExpenseManagementPartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01d58-127">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="01d58-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта telecomExpenseManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="01d58-128">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="01d58-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="01d58-129">Property</span></span>|<span data-ttu-id="01d58-130">Тип</span><span class="sxs-lookup"><span data-stu-id="01d58-130">Type</span></span>|<span data-ttu-id="01d58-131">Описание</span><span class="sxs-lookup"><span data-stu-id="01d58-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01d58-132">id</span><span class="sxs-lookup"><span data-stu-id="01d58-132">id</span></span>|<span data-ttu-id="01d58-133">String</span><span class="sxs-lookup"><span data-stu-id="01d58-133">String</span></span>|<span data-ttu-id="01d58-134">Уникальный идентификатор партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="01d58-134">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="01d58-135">displayName</span><span class="sxs-lookup"><span data-stu-id="01d58-135">displayName</span></span>|<span data-ttu-id="01d58-136">Строка</span><span class="sxs-lookup"><span data-stu-id="01d58-136">String</span></span>|<span data-ttu-id="01d58-137">Отображаемое имя партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="01d58-137">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="01d58-138">url</span><span class="sxs-lookup"><span data-stu-id="01d58-138">url</span></span>|<span data-ttu-id="01d58-139">String</span><span class="sxs-lookup"><span data-stu-id="01d58-139">String</span></span>|<span data-ttu-id="01d58-140">URL-адрес административной панели управления партнера TEM, где администратор может настроить службу TEM.</span><span class="sxs-lookup"><span data-stu-id="01d58-140">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="01d58-141">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="01d58-141">appAuthorized</span></span>|<span data-ttu-id="01d58-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="01d58-142">Boolean</span></span>|<span data-ttu-id="01d58-143">Определяет, разрешен ли доступ к Intune партнерскому приложению AAD.</span><span class="sxs-lookup"><span data-stu-id="01d58-143">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="01d58-144">enabled</span><span class="sxs-lookup"><span data-stu-id="01d58-144">enabled</span></span>|<span data-ttu-id="01d58-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="01d58-145">Boolean</span></span>|<span data-ttu-id="01d58-146">Определяет, включено или отключено сейчас подключение Intune к службе TEM.</span><span class="sxs-lookup"><span data-stu-id="01d58-146">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="01d58-147">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="01d58-147">lastConnectionDateTime</span></span>|<span data-ttu-id="01d58-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01d58-148">DateTimeOffset</span></span>|<span data-ttu-id="01d58-149">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="01d58-149">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="01d58-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="01d58-150">Response</span></span>
<span data-ttu-id="01d58-151">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="01d58-151">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01d58-152">Пример</span><span class="sxs-lookup"><span data-stu-id="01d58-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="01d58-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="01d58-153">Request</span></span>
<span data-ttu-id="01d58-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01d58-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="01d58-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="01d58-155">Response</span></span>
<span data-ttu-id="01d58-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01d58-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




