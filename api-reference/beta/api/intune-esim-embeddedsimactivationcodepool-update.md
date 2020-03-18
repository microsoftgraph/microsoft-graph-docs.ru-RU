---
title: Обновление Ембеддедсимактиватионкодепул
description: Обновление свойств объекта Ембеддедсимактиватионкодепул.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7ff74b8e0ce8728d02157bf87f0a62e1c02a77e4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804921"
---
# <a name="update-embeddedsimactivationcodepool"></a><span data-ttu-id="0e86c-103">Обновление Ембеддедсимактиватионкодепул</span><span class="sxs-lookup"><span data-stu-id="0e86c-103">Update embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="0e86c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e86c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e86c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e86c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e86c-106">Обновление свойств объекта [ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md) .</span><span class="sxs-lookup"><span data-stu-id="0e86c-106">Update the properties of a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e86c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0e86c-107">Prerequisites</span></span>
<span data-ttu-id="0e86c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e86c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e86c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e86c-110">Permission type</span></span>|<span data-ttu-id="0e86c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e86c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e86c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e86c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0e86c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e86c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e86c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e86c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e86c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e86c-115">Not supported.</span></span>|
|<span data-ttu-id="0e86c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0e86c-116">Application</span></span>|<span data-ttu-id="0e86c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e86c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e86c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e86c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="request-headers"></a><span data-ttu-id="0e86c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0e86c-119">Request headers</span></span>
|<span data-ttu-id="0e86c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e86c-120">Header</span></span>|<span data-ttu-id="0e86c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0e86c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e86c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e86c-122">Authorization</span></span>|<span data-ttu-id="0e86c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e86c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e86c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0e86c-124">Accept</span></span>|<span data-ttu-id="0e86c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0e86c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e86c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e86c-126">Request body</span></span>
<span data-ttu-id="0e86c-127">В тексте запроса добавьте представление объекта [ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e86c-127">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

<span data-ttu-id="0e86c-128">В следующей таблице приведены свойства, необходимые при создании [ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md).</span><span class="sxs-lookup"><span data-stu-id="0e86c-128">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span></span>

|<span data-ttu-id="0e86c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e86c-129">Property</span></span>|<span data-ttu-id="0e86c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0e86c-130">Type</span></span>|<span data-ttu-id="0e86c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0e86c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e86c-132">id</span><span class="sxs-lookup"><span data-stu-id="0e86c-132">id</span></span>|<span data-ttu-id="0e86c-133">String</span><span class="sxs-lookup"><span data-stu-id="0e86c-133">String</span></span>|<span data-ttu-id="0e86c-134">Уникальный идентификатор для встроенного пула кода активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="0e86c-134">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="0e86c-135">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="0e86c-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="0e86c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0e86c-136">displayName</span></span>|<span data-ttu-id="0e86c-137">Строка</span><span class="sxs-lookup"><span data-stu-id="0e86c-137">String</span></span>|<span data-ttu-id="0e86c-138">Имя администратора внедренного пула кода активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="0e86c-138">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="0e86c-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e86c-139">createdDateTime</span></span>|<span data-ttu-id="0e86c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e86c-140">DateTimeOffset</span></span>|<span data-ttu-id="0e86c-141">Время создания внедренного пула кода активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="0e86c-141">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="0e86c-142">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="0e86c-142">Generated service side.</span></span>|
|<span data-ttu-id="0e86c-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e86c-143">modifiedDateTime</span></span>|<span data-ttu-id="0e86c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e86c-144">DateTimeOffset</span></span>|<span data-ttu-id="0e86c-145">Время последнего изменения пула кода активации внедренной SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="0e86c-145">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="0e86c-146">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="0e86c-146">Updated service side.</span></span>|
|<span data-ttu-id="0e86c-147">активатионкодес</span><span class="sxs-lookup"><span data-stu-id="0e86c-147">activationCodes</span></span>|<span data-ttu-id="0e86c-148">Коллекция [ембеддедсимактиватионкоде](../resources/intune-esim-embeddedsimactivationcode.md)</span><span class="sxs-lookup"><span data-stu-id="0e86c-148">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="0e86c-149">Коды активации, принадлежащие этому пулу.</span><span class="sxs-lookup"><span data-stu-id="0e86c-149">The activation codes which belong to this pool.</span></span> <span data-ttu-id="0e86c-150">Это свойство навигации используется для публикации кодов активации в Intune, но не может использоваться для считывания кодов активации из Intune.</span><span class="sxs-lookup"><span data-stu-id="0e86c-150">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="0e86c-151">активатионкодекаунт</span><span class="sxs-lookup"><span data-stu-id="0e86c-151">activationCodeCount</span></span>|<span data-ttu-id="0e86c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0e86c-152">Int32</span></span>|<span data-ttu-id="0e86c-153">Общее количество кодов активации, относящихся к этому пулу.</span><span class="sxs-lookup"><span data-stu-id="0e86c-153">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="0e86c-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e86c-154">Response</span></span>
<span data-ttu-id="0e86c-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0e86c-155">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e86c-156">Пример</span><span class="sxs-lookup"><span data-stu-id="0e86c-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e86c-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e86c-157">Request</span></span>
<span data-ttu-id="0e86c-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e86c-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0e86c-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e86c-159">Response</span></span>
<span data-ttu-id="0e86c-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e86c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




