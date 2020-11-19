---
title: Создание Ембеддедсимактиватионкодепул
description: Создание нового объекта Ембеддедсимактиватионкодепул.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bb268bfc34e55829b7de593a58d5e2cdb4932a98
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49218406"
---
# <a name="create-embeddedsimactivationcodepool"></a><span data-ttu-id="f77ac-103">Создание Ембеддедсимактиватионкодепул</span><span class="sxs-lookup"><span data-stu-id="f77ac-103">Create embeddedSIMActivationCodePool</span></span>

<span data-ttu-id="f77ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f77ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f77ac-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f77ac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f77ac-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f77ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f77ac-107">Создание нового объекта [ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md) .</span><span class="sxs-lookup"><span data-stu-id="f77ac-107">Create a new [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f77ac-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f77ac-108">Prerequisites</span></span>
<span data-ttu-id="f77ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f77ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f77ac-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f77ac-111">Permission type</span></span>|<span data-ttu-id="f77ac-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f77ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f77ac-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f77ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f77ac-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f77ac-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f77ac-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f77ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f77ac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f77ac-116">Not supported.</span></span>|
|<span data-ttu-id="f77ac-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f77ac-117">Application</span></span>|<span data-ttu-id="f77ac-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f77ac-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f77ac-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f77ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools
```

## <a name="request-headers"></a><span data-ttu-id="f77ac-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f77ac-120">Request headers</span></span>
|<span data-ttu-id="f77ac-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f77ac-121">Header</span></span>|<span data-ttu-id="f77ac-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f77ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f77ac-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f77ac-123">Authorization</span></span>|<span data-ttu-id="f77ac-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f77ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f77ac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f77ac-125">Accept</span></span>|<span data-ttu-id="f77ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f77ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f77ac-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f77ac-127">Request body</span></span>
<span data-ttu-id="f77ac-128">В тексте запроса добавьте представление объекта Ембеддедсимактиватионкодепул в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f77ac-128">In the request body, supply a JSON representation for the embeddedSIMActivationCodePool object.</span></span>

<span data-ttu-id="f77ac-129">В следующей таблице приведены свойства, необходимые при создании Ембеддедсимактиватионкодепул.</span><span class="sxs-lookup"><span data-stu-id="f77ac-129">The following table shows the properties that are required when you create the embeddedSIMActivationCodePool.</span></span>

|<span data-ttu-id="f77ac-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f77ac-130">Property</span></span>|<span data-ttu-id="f77ac-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f77ac-131">Type</span></span>|<span data-ttu-id="f77ac-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f77ac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f77ac-133">id</span><span class="sxs-lookup"><span data-stu-id="f77ac-133">id</span></span>|<span data-ttu-id="f77ac-134">String</span><span class="sxs-lookup"><span data-stu-id="f77ac-134">String</span></span>|<span data-ttu-id="f77ac-135">Уникальный идентификатор для встроенного пула кода активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="f77ac-135">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="f77ac-136">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="f77ac-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="f77ac-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f77ac-137">displayName</span></span>|<span data-ttu-id="f77ac-138">String</span><span class="sxs-lookup"><span data-stu-id="f77ac-138">String</span></span>|<span data-ttu-id="f77ac-139">Имя администратора внедренного пула кода активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="f77ac-139">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="f77ac-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f77ac-140">createdDateTime</span></span>|<span data-ttu-id="f77ac-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f77ac-141">DateTimeOffset</span></span>|<span data-ttu-id="f77ac-142">Время создания внедренного пула кода активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="f77ac-142">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="f77ac-143">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="f77ac-143">Generated service side.</span></span>|
|<span data-ttu-id="f77ac-144">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f77ac-144">modifiedDateTime</span></span>|<span data-ttu-id="f77ac-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f77ac-145">DateTimeOffset</span></span>|<span data-ttu-id="f77ac-146">Время последнего изменения пула кода активации внедренной SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="f77ac-146">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="f77ac-147">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="f77ac-147">Updated service side.</span></span>|
|<span data-ttu-id="f77ac-148">активатионкодес</span><span class="sxs-lookup"><span data-stu-id="f77ac-148">activationCodes</span></span>|<span data-ttu-id="f77ac-149">Коллекция [ембеддедсимактиватионкоде](../resources/intune-esim-embeddedsimactivationcode.md)</span><span class="sxs-lookup"><span data-stu-id="f77ac-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="f77ac-150">Коды активации, принадлежащие этому пулу.</span><span class="sxs-lookup"><span data-stu-id="f77ac-150">The activation codes which belong to this pool.</span></span> <span data-ttu-id="f77ac-151">Это свойство навигации используется для публикации кодов активации в Intune, но не может использоваться для считывания кодов активации из Intune.</span><span class="sxs-lookup"><span data-stu-id="f77ac-151">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="f77ac-152">активатионкодекаунт</span><span class="sxs-lookup"><span data-stu-id="f77ac-152">activationCodeCount</span></span>|<span data-ttu-id="f77ac-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f77ac-153">Int32</span></span>|<span data-ttu-id="f77ac-154">Общее количество кодов активации, относящихся к этому пулу.</span><span class="sxs-lookup"><span data-stu-id="f77ac-154">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="f77ac-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="f77ac-155">Response</span></span>
<span data-ttu-id="f77ac-156">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f77ac-156">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f77ac-157">Пример</span><span class="sxs-lookup"><span data-stu-id="f77ac-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="f77ac-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="f77ac-158">Request</span></span>
<span data-ttu-id="f77ac-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f77ac-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f77ac-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="f77ac-160">Response</span></span>
<span data-ttu-id="f77ac-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f77ac-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




