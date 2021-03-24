---
title: Обновление встроенныхSIMActivationCodePool
description: Обновление свойств встроенного объектаSIMActivationCodePool.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: be9d88f6f75d677cf3b8133e8e094da2f1c09dda
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126131"
---
# <a name="update-embeddedsimactivationcodepool"></a><span data-ttu-id="d9e4c-103">Обновление встроенныхSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="d9e4c-103">Update embeddedSIMActivationCodePool</span></span>

<span data-ttu-id="d9e4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9e4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9e4c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9e4c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9e4c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9e4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9e4c-107">Обновление свойств встроенного [объектаSIMActivationCodePool.](../resources/intune-esim-embeddedsimactivationcodepool.md)</span><span class="sxs-lookup"><span data-stu-id="d9e4c-107">Update the properties of a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9e4c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d9e4c-108">Prerequisites</span></span>
<span data-ttu-id="d9e4c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9e4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9e4c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9e4c-111">Permission type</span></span>|<span data-ttu-id="d9e4c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9e4c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9e4c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9e4c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9e4c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9e4c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d9e4c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9e4c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9e4c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9e4c-116">Not supported.</span></span>|
|<span data-ttu-id="d9e4c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d9e4c-117">Application</span></span>|<span data-ttu-id="d9e4c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9e4c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9e4c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9e4c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="request-headers"></a><span data-ttu-id="d9e4c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d9e4c-120">Request headers</span></span>
|<span data-ttu-id="d9e4c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d9e4c-121">Header</span></span>|<span data-ttu-id="d9e4c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d9e4c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9e4c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9e4c-123">Authorization</span></span>|<span data-ttu-id="d9e4c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9e4c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9e4c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d9e4c-125">Accept</span></span>|<span data-ttu-id="d9e4c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9e4c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9e4c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9e4c-127">Request body</span></span>
<span data-ttu-id="d9e4c-128">В теле запроса поставляем представление JSON для встроенного [объектаSIMActivationCodePool.](../resources/intune-esim-embeddedsimactivationcodepool.md)</span><span class="sxs-lookup"><span data-stu-id="d9e4c-128">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

<span data-ttu-id="d9e4c-129">В следующей таблице показаны свойства, необходимые при создании [встроенногоSIMActivationCodePool.](../resources/intune-esim-embeddedsimactivationcodepool.md)</span><span class="sxs-lookup"><span data-stu-id="d9e4c-129">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span></span>

|<span data-ttu-id="d9e4c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9e4c-130">Property</span></span>|<span data-ttu-id="d9e4c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d9e4c-131">Type</span></span>|<span data-ttu-id="d9e4c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d9e4c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9e4c-133">id</span><span class="sxs-lookup"><span data-stu-id="d9e4c-133">id</span></span>|<span data-ttu-id="d9e4c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d9e4c-134">String</span></span>|<span data-ttu-id="d9e4c-135">Уникальный идентификатор встроенного пула кодов активации SIM.</span><span class="sxs-lookup"><span data-stu-id="d9e4c-135">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="d9e4c-136">Созданное в системе значение, назначенное при его создания.</span><span class="sxs-lookup"><span data-stu-id="d9e4c-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="d9e4c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d9e4c-137">displayName</span></span>|<span data-ttu-id="d9e4c-138">Строка</span><span class="sxs-lookup"><span data-stu-id="d9e4c-138">String</span></span>|<span data-ttu-id="d9e4c-139">Администратор определил имя встроенного пула кодов активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="d9e4c-139">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="d9e4c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9e4c-140">createdDateTime</span></span>|<span data-ttu-id="d9e4c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9e4c-141">DateTimeOffset</span></span>|<span data-ttu-id="d9e4c-142">Время создания встроенного пула кодов активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="d9e4c-142">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="d9e4c-143">Сгенерированная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="d9e4c-143">Generated service side.</span></span>|
|<span data-ttu-id="d9e4c-144">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9e4c-144">modifiedDateTime</span></span>|<span data-ttu-id="d9e4c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9e4c-145">DateTimeOffset</span></span>|<span data-ttu-id="d9e4c-146">Время последнего изменения встроенного пула кодов активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="d9e4c-146">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="d9e4c-147">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="d9e4c-147">Updated service side.</span></span>|
|<span data-ttu-id="d9e4c-148">activationCodes</span><span class="sxs-lookup"><span data-stu-id="d9e4c-148">activationCodes</span></span>|<span data-ttu-id="d9e4c-149">[коллекция embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)</span><span class="sxs-lookup"><span data-stu-id="d9e4c-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="d9e4c-150">Коды активации, которые принадлежат этому пулу.</span><span class="sxs-lookup"><span data-stu-id="d9e4c-150">The activation codes which belong to this pool.</span></span> <span data-ttu-id="d9e4c-151">Это свойство навигации используется для публикации кодов активации в Intune, но не может использоваться для чтения кодов активации из Intune.</span><span class="sxs-lookup"><span data-stu-id="d9e4c-151">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="d9e4c-152">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="d9e4c-152">activationCodeCount</span></span>|<span data-ttu-id="d9e4c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="d9e4c-153">Int32</span></span>|<span data-ttu-id="d9e4c-154">Общее количество кодов активации, которые относятся к этому пулу.</span><span class="sxs-lookup"><span data-stu-id="d9e4c-154">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="d9e4c-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9e4c-155">Response</span></span>
<span data-ttu-id="d9e4c-156">В случае успеха этот метод возвращает код отклика и обновленный встроенный `200 OK` [объектSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d9e4c-156">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9e4c-157">Пример</span><span class="sxs-lookup"><span data-stu-id="d9e4c-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9e4c-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9e4c-158">Request</span></span>
<span data-ttu-id="d9e4c-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9e4c-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
Content-type: application/json
Content-length: 460

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "displayName": "Display Name value",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```

### <a name="response"></a><span data-ttu-id="d9e4c-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9e4c-160">Response</span></span>
<span data-ttu-id="d9e4c-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9e4c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 628

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "ec308741-8741-ec30-4187-30ec418730ec",
  "displayName": "Display Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```




