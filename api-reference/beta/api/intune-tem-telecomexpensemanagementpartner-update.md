---
title: Обновление объекта telecomExpenseManagementPartner
description: Обновление свойств объекта telecomExpenseManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94b9ac0e0456d80a53d937a025084ffd7a28affe
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983045"
---
# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="880c3-103">Обновление объекта telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="880c3-103">Update telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="880c3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="880c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="880c3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="880c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="880c3-106">Обновление свойств объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="880c3-106">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="880c3-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="880c3-107">Prerequisites</span></span>
<span data-ttu-id="880c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="880c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="880c3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="880c3-110">Permission type</span></span>|<span data-ttu-id="880c3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="880c3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="880c3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="880c3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="880c3-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="880c3-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="880c3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="880c3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="880c3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="880c3-115">Not supported.</span></span>|
|<span data-ttu-id="880c3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="880c3-116">Application</span></span>|<span data-ttu-id="880c3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="880c3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="880c3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="880c3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="880c3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="880c3-119">Request headers</span></span>
|<span data-ttu-id="880c3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="880c3-120">Header</span></span>|<span data-ttu-id="880c3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="880c3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="880c3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="880c3-122">Authorization</span></span>|<span data-ttu-id="880c3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="880c3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="880c3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="880c3-124">Accept</span></span>|<span data-ttu-id="880c3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="880c3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="880c3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="880c3-126">Request body</span></span>
<span data-ttu-id="880c3-127">В теле запроса добавьте представление объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="880c3-127">In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="880c3-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="880c3-128">The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>

|<span data-ttu-id="880c3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="880c3-129">Property</span></span>|<span data-ttu-id="880c3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="880c3-130">Type</span></span>|<span data-ttu-id="880c3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="880c3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="880c3-132">id</span><span class="sxs-lookup"><span data-stu-id="880c3-132">id</span></span>|<span data-ttu-id="880c3-133">String</span><span class="sxs-lookup"><span data-stu-id="880c3-133">String</span></span>|<span data-ttu-id="880c3-134">Уникальный идентификатор партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="880c3-134">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="880c3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="880c3-135">displayName</span></span>|<span data-ttu-id="880c3-136">Строка</span><span class="sxs-lookup"><span data-stu-id="880c3-136">String</span></span>|<span data-ttu-id="880c3-137">Отображаемое имя партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="880c3-137">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="880c3-138">url</span><span class="sxs-lookup"><span data-stu-id="880c3-138">url</span></span>|<span data-ttu-id="880c3-139">String</span><span class="sxs-lookup"><span data-stu-id="880c3-139">String</span></span>|<span data-ttu-id="880c3-140">URL-адрес административной панели управления партнера TEM, где администратор может настроить службу TEM.</span><span class="sxs-lookup"><span data-stu-id="880c3-140">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="880c3-141">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="880c3-141">appAuthorized</span></span>|<span data-ttu-id="880c3-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="880c3-142">Boolean</span></span>|<span data-ttu-id="880c3-143">Определяет, разрешен ли доступ к Intune партнерскому приложению AAD.</span><span class="sxs-lookup"><span data-stu-id="880c3-143">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="880c3-144">enabled</span><span class="sxs-lookup"><span data-stu-id="880c3-144">enabled</span></span>|<span data-ttu-id="880c3-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="880c3-145">Boolean</span></span>|<span data-ttu-id="880c3-146">Определяет, включено или отключено сейчас подключение Intune к службе TEM.</span><span class="sxs-lookup"><span data-stu-id="880c3-146">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="880c3-147">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="880c3-147">lastConnectionDateTime</span></span>|<span data-ttu-id="880c3-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="880c3-148">DateTimeOffset</span></span>|<span data-ttu-id="880c3-149">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="880c3-149">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="880c3-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="880c3-150">Response</span></span>
<span data-ttu-id="880c3-151">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="880c3-151">If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="880c3-152">Пример</span><span class="sxs-lookup"><span data-stu-id="880c3-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="880c3-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="880c3-153">Request</span></span>
<span data-ttu-id="880c3-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="880c3-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
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

### <a name="response"></a><span data-ttu-id="880c3-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="880c3-155">Response</span></span>
<span data-ttu-id="880c3-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="880c3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




