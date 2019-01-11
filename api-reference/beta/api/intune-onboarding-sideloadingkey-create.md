---
title: Создание sideLoadingKey
description: Создание нового объекта sideLoadingKey.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 178236e03d508eb8a5017b67a1795fceca72bdee
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838873"
---
# <a name="create-sideloadingkey"></a><span data-ttu-id="46778-103">Создание sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="46778-103">Create sideLoadingKey</span></span>

> <span data-ttu-id="46778-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="46778-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46778-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46778-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46778-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="46778-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46778-107">Создание нового объекта [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="46778-107">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="46778-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="46778-108">Prerequisites</span></span>
<span data-ttu-id="46778-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46778-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46778-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46778-111">Permission type</span></span>|<span data-ttu-id="46778-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46778-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46778-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46778-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46778-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46778-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="46778-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46778-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46778-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46778-116">Not supported.</span></span>|
|<span data-ttu-id="46778-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46778-117">Application</span></span>|<span data-ttu-id="46778-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46778-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46778-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46778-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="46778-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46778-120">Request headers</span></span>
|<span data-ttu-id="46778-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46778-121">Header</span></span>|<span data-ttu-id="46778-122">Значение</span><span class="sxs-lookup"><span data-stu-id="46778-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46778-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="46778-123">Authorization</span></span>|<span data-ttu-id="46778-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="46778-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46778-125">Accept</span><span class="sxs-lookup"><span data-stu-id="46778-125">Accept</span></span>|<span data-ttu-id="46778-126">application/json</span><span class="sxs-lookup"><span data-stu-id="46778-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46778-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="46778-127">Request body</span></span>
<span data-ttu-id="46778-128">В тексте запроса укажите представление JSON для объекта sideLoadingKey.</span><span class="sxs-lookup"><span data-stu-id="46778-128">In the request body, supply a JSON representation for the sideLoadingKey object.</span></span>

<span data-ttu-id="46778-129">В следующей таблице показаны свойства, которые необходимы для создания sideLoadingKey.</span><span class="sxs-lookup"><span data-stu-id="46778-129">The following table shows the properties that are required when you create the sideLoadingKey.</span></span>

|<span data-ttu-id="46778-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="46778-130">Property</span></span>|<span data-ttu-id="46778-131">Тип</span><span class="sxs-lookup"><span data-stu-id="46778-131">Type</span></span>|<span data-ttu-id="46778-132">Описание</span><span class="sxs-lookup"><span data-stu-id="46778-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46778-133">id</span><span class="sxs-lookup"><span data-stu-id="46778-133">id</span></span>|<span data-ttu-id="46778-134">Строка</span><span class="sxs-lookup"><span data-stu-id="46778-134">String</span></span>|<span data-ttu-id="46778-135">Со стороны загрузка уникальный идентификатор ключа.</span><span class="sxs-lookup"><span data-stu-id="46778-135">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="46778-136">value</span><span class="sxs-lookup"><span data-stu-id="46778-136">value</span></span>|<span data-ttu-id="46778-137">Строка</span><span class="sxs-lookup"><span data-stu-id="46778-137">String</span></span>|<span data-ttu-id="46778-138">Со стороны загрузки ключ значение — значение 5 x 5, разделенных hiphens.</span><span class="sxs-lookup"><span data-stu-id="46778-138">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="46778-139">displayName</span><span class="sxs-lookup"><span data-stu-id="46778-139">displayName</span></span>|<span data-ttu-id="46778-140">Строка</span><span class="sxs-lookup"><span data-stu-id="46778-140">String</span></span>|<span data-ttu-id="46778-141">Со стороны загрузка ключа имя, отображаемое для администраторов для ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="46778-141">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="46778-142">описание</span><span class="sxs-lookup"><span data-stu-id="46778-142">description</span></span>|<span data-ttu-id="46778-143">Строка</span><span class="sxs-lookup"><span data-stu-id="46778-143">String</span></span>|<span data-ttu-id="46778-144">Со стороны загрузки ключ описание, отображаемое для администраторов для ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="46778-144">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="46778-145">totalActivation</span><span class="sxs-lookup"><span data-stu-id="46778-145">totalActivation</span></span>|<span data-ttu-id="46778-146">Int32</span><span class="sxs-lookup"><span data-stu-id="46778-146">Int32</span></span>|<span data-ttu-id="46778-147">Со стороны загрузки ключ общее активация отображаются для администраторов для ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="46778-147">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="46778-148">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="46778-148">lastUpdatedDateTime</span></span>|<span data-ttu-id="46778-149">Строка</span><span class="sxs-lookup"><span data-stu-id="46778-149">String</span></span>|<span data-ttu-id="46778-150">Со стороны загрузки ключ обновлен Дата последнего отображаются для администраторов для ИТ-специалистов.</span><span class="sxs-lookup"><span data-stu-id="46778-150">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="46778-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="46778-151">Response</span></span>
<span data-ttu-id="46778-152">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="46778-152">If successful, this method returns a `201 Created` response code and a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46778-153">Пример</span><span class="sxs-lookup"><span data-stu-id="46778-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="46778-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="46778-154">Request</span></span>
<span data-ttu-id="46778-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46778-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys
Content-type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

### <a name="response"></a><span data-ttu-id="46778-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="46778-156">Response</span></span>
<span data-ttu-id="46778-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="46778-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```





