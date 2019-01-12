---
title: Создание telecomExpenseManagementPartner
description: Создание объекта telecomExpenseManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 326454d9517839096261624617113d7b190a2308
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919836"
---
# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="6396c-103">Создание telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="6396c-103">Create telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="6396c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6396c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6396c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6396c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6396c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6396c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6396c-107">Создание объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="6396c-107">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6396c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6396c-108">Prerequisites</span></span>
<span data-ttu-id="6396c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6396c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6396c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6396c-111">Permission type</span></span>|<span data-ttu-id="6396c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6396c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6396c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6396c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6396c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6396c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6396c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6396c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6396c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6396c-116">Not supported.</span></span>|
|<span data-ttu-id="6396c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6396c-117">Application</span></span>|<span data-ttu-id="6396c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6396c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6396c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6396c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="6396c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6396c-120">Request headers</span></span>
|<span data-ttu-id="6396c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6396c-121">Header</span></span>|<span data-ttu-id="6396c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6396c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6396c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6396c-123">Authorization</span></span>|<span data-ttu-id="6396c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6396c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6396c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6396c-125">Accept</span></span>|<span data-ttu-id="6396c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6396c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6396c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6396c-127">Request body</span></span>
<span data-ttu-id="6396c-128">В теле запроса добавьте представление объекта telecomExpenseManagementPartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6396c-128">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="6396c-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта telecomExpenseManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="6396c-129">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="6396c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6396c-130">Property</span></span>|<span data-ttu-id="6396c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6396c-131">Type</span></span>|<span data-ttu-id="6396c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6396c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6396c-133">id</span><span class="sxs-lookup"><span data-stu-id="6396c-133">id</span></span>|<span data-ttu-id="6396c-134">String</span><span class="sxs-lookup"><span data-stu-id="6396c-134">String</span></span>|<span data-ttu-id="6396c-135">Уникальный идентификатор партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="6396c-135">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="6396c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6396c-136">displayName</span></span>|<span data-ttu-id="6396c-137">String</span><span class="sxs-lookup"><span data-stu-id="6396c-137">String</span></span>|<span data-ttu-id="6396c-138">Отображаемое имя партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="6396c-138">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="6396c-139">url</span><span class="sxs-lookup"><span data-stu-id="6396c-139">url</span></span>|<span data-ttu-id="6396c-140">String</span><span class="sxs-lookup"><span data-stu-id="6396c-140">String</span></span>|<span data-ttu-id="6396c-141">URL-адрес административной панели управления партнера TEM, где администратор может настроить службу TEM.</span><span class="sxs-lookup"><span data-stu-id="6396c-141">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="6396c-142">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="6396c-142">appAuthorized</span></span>|<span data-ttu-id="6396c-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="6396c-143">Boolean</span></span>|<span data-ttu-id="6396c-144">Определяет, разрешен ли доступ к Intune партнерскому приложению AAD.</span><span class="sxs-lookup"><span data-stu-id="6396c-144">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="6396c-145">enabled</span><span class="sxs-lookup"><span data-stu-id="6396c-145">enabled</span></span>|<span data-ttu-id="6396c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6396c-146">Boolean</span></span>|<span data-ttu-id="6396c-147">Определяет, включено или отключено сейчас подключение Intune к службе TEM.</span><span class="sxs-lookup"><span data-stu-id="6396c-147">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="6396c-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="6396c-148">lastConnectionDateTime</span></span>|<span data-ttu-id="6396c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6396c-149">DateTimeOffset</span></span>|<span data-ttu-id="6396c-150">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="6396c-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="6396c-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="6396c-151">Response</span></span>
<span data-ttu-id="6396c-152">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6396c-152">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6396c-153">Пример</span><span class="sxs-lookup"><span data-stu-id="6396c-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="6396c-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="6396c-154">Request</span></span>
<span data-ttu-id="6396c-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6396c-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6396c-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="6396c-156">Response</span></span>
<span data-ttu-id="6396c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6396c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





