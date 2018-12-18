---
title: Создание telecomExpenseManagementPartner
description: Создание объекта telecomExpenseManagementPartner.
author: tfitzmac
ms.openlocfilehash: e3b099bf71b586313a5cf67012c7f24ebc7e858c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322409"
---
# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="e9b13-103">Создание telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="e9b13-103">Create telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="e9b13-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e9b13-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9b13-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9b13-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e9b13-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e9b13-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9b13-107">Создание объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="e9b13-107">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e9b13-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e9b13-108">Prerequisites</span></span>
<span data-ttu-id="e9b13-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9b13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9b13-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9b13-111">Permission type</span></span>|<span data-ttu-id="e9b13-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9b13-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9b13-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9b13-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9b13-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9b13-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e9b13-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9b13-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9b13-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9b13-116">Not supported.</span></span>|
|<span data-ttu-id="e9b13-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9b13-117">Application</span></span>|<span data-ttu-id="e9b13-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9b13-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9b13-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9b13-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="e9b13-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9b13-120">Request headers</span></span>
|<span data-ttu-id="e9b13-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e9b13-121">Header</span></span>|<span data-ttu-id="e9b13-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e9b13-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9b13-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9b13-123">Authorization</span></span>|<span data-ttu-id="e9b13-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e9b13-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9b13-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e9b13-125">Accept</span></span>|<span data-ttu-id="e9b13-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9b13-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9b13-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e9b13-127">Request body</span></span>
<span data-ttu-id="e9b13-128">В теле запроса добавьте представление объекта telecomExpenseManagementPartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9b13-128">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="e9b13-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта telecomExpenseManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="e9b13-129">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="e9b13-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9b13-130">Property</span></span>|<span data-ttu-id="e9b13-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e9b13-131">Type</span></span>|<span data-ttu-id="e9b13-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e9b13-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9b13-133">id</span><span class="sxs-lookup"><span data-stu-id="e9b13-133">id</span></span>|<span data-ttu-id="e9b13-134">String</span><span class="sxs-lookup"><span data-stu-id="e9b13-134">String</span></span>|<span data-ttu-id="e9b13-135">Уникальный идентификатор партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="e9b13-135">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="e9b13-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e9b13-136">displayName</span></span>|<span data-ttu-id="e9b13-137">String</span><span class="sxs-lookup"><span data-stu-id="e9b13-137">String</span></span>|<span data-ttu-id="e9b13-138">Отображаемое имя партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="e9b13-138">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="e9b13-139">url</span><span class="sxs-lookup"><span data-stu-id="e9b13-139">url</span></span>|<span data-ttu-id="e9b13-140">String</span><span class="sxs-lookup"><span data-stu-id="e9b13-140">String</span></span>|<span data-ttu-id="e9b13-141">URL-адрес административной панели управления партнера TEM, где администратор может настроить службу TEM.</span><span class="sxs-lookup"><span data-stu-id="e9b13-141">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="e9b13-142">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="e9b13-142">appAuthorized</span></span>|<span data-ttu-id="e9b13-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9b13-143">Boolean</span></span>|<span data-ttu-id="e9b13-144">Определяет, разрешен ли доступ к Intune партнерскому приложению AAD.</span><span class="sxs-lookup"><span data-stu-id="e9b13-144">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="e9b13-145">enabled</span><span class="sxs-lookup"><span data-stu-id="e9b13-145">enabled</span></span>|<span data-ttu-id="e9b13-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9b13-146">Boolean</span></span>|<span data-ttu-id="e9b13-147">Определяет, включено или отключено сейчас подключение Intune к службе TEM.</span><span class="sxs-lookup"><span data-stu-id="e9b13-147">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="e9b13-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="e9b13-148">lastConnectionDateTime</span></span>|<span data-ttu-id="e9b13-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9b13-149">DateTimeOffset</span></span>|<span data-ttu-id="e9b13-150">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="e9b13-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="e9b13-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9b13-151">Response</span></span>
<span data-ttu-id="e9b13-152">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e9b13-152">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9b13-153">Пример</span><span class="sxs-lookup"><span data-stu-id="e9b13-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="e9b13-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9b13-154">Request</span></span>
<span data-ttu-id="e9b13-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9b13-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e9b13-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9b13-156">Response</span></span>
<span data-ttu-id="e9b13-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e9b13-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





