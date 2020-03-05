---
title: Создание Ембеддедсимактиватионкодепул
description: Создание нового объекта Ембеддедсимактиватионкодепул.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d018340411613fb0f5ccf9d17ed62a207559e19e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42466138"
---
# <a name="create-embeddedsimactivationcodepool"></a><span data-ttu-id="ae6b3-103">Создание Ембеддедсимактиватионкодепул</span><span class="sxs-lookup"><span data-stu-id="ae6b3-103">Create embeddedSIMActivationCodePool</span></span>

<span data-ttu-id="ae6b3-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ae6b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae6b3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae6b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae6b3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae6b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae6b3-107">Создание нового объекта [ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md) .</span><span class="sxs-lookup"><span data-stu-id="ae6b3-107">Create a new [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae6b3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ae6b3-108">Prerequisites</span></span>
<span data-ttu-id="ae6b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae6b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae6b3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae6b3-111">Permission type</span></span>|<span data-ttu-id="ae6b3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae6b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae6b3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae6b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae6b3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae6b3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae6b3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae6b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae6b3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae6b3-116">Not supported.</span></span>|
|<span data-ttu-id="ae6b3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae6b3-117">Application</span></span>|<span data-ttu-id="ae6b3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae6b3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae6b3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae6b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools
```

## <a name="request-headers"></a><span data-ttu-id="ae6b3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ae6b3-120">Request headers</span></span>
|<span data-ttu-id="ae6b3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ae6b3-121">Header</span></span>|<span data-ttu-id="ae6b3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ae6b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae6b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae6b3-123">Authorization</span></span>|<span data-ttu-id="ae6b3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae6b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae6b3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ae6b3-125">Accept</span></span>|<span data-ttu-id="ae6b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae6b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae6b3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae6b3-127">Request body</span></span>
<span data-ttu-id="ae6b3-128">В тексте запроса добавьте представление объекта Ембеддедсимактиватионкодепул в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae6b3-128">In the request body, supply a JSON representation for the embeddedSIMActivationCodePool object.</span></span>

<span data-ttu-id="ae6b3-129">В следующей таблице приведены свойства, необходимые при создании Ембеддедсимактиватионкодепул.</span><span class="sxs-lookup"><span data-stu-id="ae6b3-129">The following table shows the properties that are required when you create the embeddedSIMActivationCodePool.</span></span>

|<span data-ttu-id="ae6b3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae6b3-130">Property</span></span>|<span data-ttu-id="ae6b3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ae6b3-131">Type</span></span>|<span data-ttu-id="ae6b3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ae6b3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae6b3-133">id</span><span class="sxs-lookup"><span data-stu-id="ae6b3-133">id</span></span>|<span data-ttu-id="ae6b3-134">String</span><span class="sxs-lookup"><span data-stu-id="ae6b3-134">String</span></span>|<span data-ttu-id="ae6b3-135">Уникальный идентификатор для встроенного пула кода активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="ae6b3-135">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="ae6b3-136">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="ae6b3-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="ae6b3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ae6b3-137">displayName</span></span>|<span data-ttu-id="ae6b3-138">Строка</span><span class="sxs-lookup"><span data-stu-id="ae6b3-138">String</span></span>|<span data-ttu-id="ae6b3-139">Имя администратора внедренного пула кода активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="ae6b3-139">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="ae6b3-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae6b3-140">createdDateTime</span></span>|<span data-ttu-id="ae6b3-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae6b3-141">DateTimeOffset</span></span>|<span data-ttu-id="ae6b3-142">Время создания внедренного пула кода активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="ae6b3-142">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="ae6b3-143">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="ae6b3-143">Generated service side.</span></span>|
|<span data-ttu-id="ae6b3-144">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae6b3-144">modifiedDateTime</span></span>|<span data-ttu-id="ae6b3-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae6b3-145">DateTimeOffset</span></span>|<span data-ttu-id="ae6b3-146">Время последнего изменения пула кода активации внедренной SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="ae6b3-146">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="ae6b3-147">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="ae6b3-147">Updated service side.</span></span>|
|<span data-ttu-id="ae6b3-148">активатионкодес</span><span class="sxs-lookup"><span data-stu-id="ae6b3-148">activationCodes</span></span>|<span data-ttu-id="ae6b3-149">Коллекция [ембеддедсимактиватионкоде](../resources/intune-esim-embeddedsimactivationcode.md)</span><span class="sxs-lookup"><span data-stu-id="ae6b3-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="ae6b3-150">Коды активации, принадлежащие этому пулу.</span><span class="sxs-lookup"><span data-stu-id="ae6b3-150">The activation codes which belong to this pool.</span></span> <span data-ttu-id="ae6b3-151">Это свойство навигации используется для публикации кодов активации в Intune, но не может использоваться для считывания кодов активации из Intune.</span><span class="sxs-lookup"><span data-stu-id="ae6b3-151">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="ae6b3-152">активатионкодекаунт</span><span class="sxs-lookup"><span data-stu-id="ae6b3-152">activationCodeCount</span></span>|<span data-ttu-id="ae6b3-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ae6b3-153">Int32</span></span>|<span data-ttu-id="ae6b3-154">Общее количество кодов активации, относящихся к этому пулу.</span><span class="sxs-lookup"><span data-stu-id="ae6b3-154">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="ae6b3-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae6b3-155">Response</span></span>
<span data-ttu-id="ae6b3-156">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ae6b3-156">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae6b3-157">Пример</span><span class="sxs-lookup"><span data-stu-id="ae6b3-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae6b3-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae6b3-158">Request</span></span>
<span data-ttu-id="ae6b3-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae6b3-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools
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

### <a name="response"></a><span data-ttu-id="ae6b3-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae6b3-160">Response</span></span>
<span data-ttu-id="ae6b3-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae6b3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





