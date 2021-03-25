---
title: Создание встроенныхSIMActivationCodePool
description: Создайте новый встроенный объектSIMActivationCodePool.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 567bd02f6a3d39d26ba228bdc12ff6f23b03aae5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157620"
---
# <a name="create-embeddedsimactivationcodepool"></a><span data-ttu-id="a710a-103">Создание встроенныхSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="a710a-103">Create embeddedSIMActivationCodePool</span></span>

<span data-ttu-id="a710a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a710a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a710a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a710a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a710a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a710a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a710a-107">Создайте новый [встроенный объектSIMActivationCodePool.](../resources/intune-esim-embeddedsimactivationcodepool.md)</span><span class="sxs-lookup"><span data-stu-id="a710a-107">Create a new [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a710a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a710a-108">Prerequisites</span></span>
<span data-ttu-id="a710a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a710a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a710a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a710a-111">Permission type</span></span>|<span data-ttu-id="a710a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a710a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a710a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a710a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a710a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a710a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a710a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a710a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a710a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a710a-116">Not supported.</span></span>|
|<span data-ttu-id="a710a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a710a-117">Application</span></span>|<span data-ttu-id="a710a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a710a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a710a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a710a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools
```

## <a name="request-headers"></a><span data-ttu-id="a710a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a710a-120">Request headers</span></span>
|<span data-ttu-id="a710a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a710a-121">Header</span></span>|<span data-ttu-id="a710a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a710a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a710a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a710a-123">Authorization</span></span>|<span data-ttu-id="a710a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a710a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a710a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a710a-125">Accept</span></span>|<span data-ttu-id="a710a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a710a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a710a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a710a-127">Request body</span></span>
<span data-ttu-id="a710a-128">В теле запроса поставляем представление JSON для встроенного объектаSIMActivationCodePool.</span><span class="sxs-lookup"><span data-stu-id="a710a-128">In the request body, supply a JSON representation for the embeddedSIMActivationCodePool object.</span></span>

<span data-ttu-id="a710a-129">В следующей таблице показаны свойства, необходимые при создании встроенногоSIMActivationCodePool.</span><span class="sxs-lookup"><span data-stu-id="a710a-129">The following table shows the properties that are required when you create the embeddedSIMActivationCodePool.</span></span>

|<span data-ttu-id="a710a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a710a-130">Property</span></span>|<span data-ttu-id="a710a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a710a-131">Type</span></span>|<span data-ttu-id="a710a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a710a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a710a-133">id</span><span class="sxs-lookup"><span data-stu-id="a710a-133">id</span></span>|<span data-ttu-id="a710a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a710a-134">String</span></span>|<span data-ttu-id="a710a-135">Уникальный идентификатор встроенного пула кодов активации SIM.</span><span class="sxs-lookup"><span data-stu-id="a710a-135">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="a710a-136">Созданное в системе значение, назначенное при его создания.</span><span class="sxs-lookup"><span data-stu-id="a710a-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="a710a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a710a-137">displayName</span></span>|<span data-ttu-id="a710a-138">Строка</span><span class="sxs-lookup"><span data-stu-id="a710a-138">String</span></span>|<span data-ttu-id="a710a-139">Администратор определил имя встроенного пула кодов активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="a710a-139">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="a710a-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a710a-140">createdDateTime</span></span>|<span data-ttu-id="a710a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a710a-141">DateTimeOffset</span></span>|<span data-ttu-id="a710a-142">Время создания встроенного пула кодов активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="a710a-142">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="a710a-143">Сгенерированная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="a710a-143">Generated service side.</span></span>|
|<span data-ttu-id="a710a-144">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a710a-144">modifiedDateTime</span></span>|<span data-ttu-id="a710a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a710a-145">DateTimeOffset</span></span>|<span data-ttu-id="a710a-146">Время последнего изменения встроенного пула кодов активации SIM-карты.</span><span class="sxs-lookup"><span data-stu-id="a710a-146">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="a710a-147">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="a710a-147">Updated service side.</span></span>|
|<span data-ttu-id="a710a-148">activationCodes</span><span class="sxs-lookup"><span data-stu-id="a710a-148">activationCodes</span></span>|<span data-ttu-id="a710a-149">[коллекция embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)</span><span class="sxs-lookup"><span data-stu-id="a710a-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="a710a-150">Коды активации, которые принадлежат этому пулу.</span><span class="sxs-lookup"><span data-stu-id="a710a-150">The activation codes which belong to this pool.</span></span> <span data-ttu-id="a710a-151">Это свойство навигации используется для публикации кодов активации в Intune, но не может использоваться для чтения кодов активации из Intune.</span><span class="sxs-lookup"><span data-stu-id="a710a-151">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="a710a-152">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="a710a-152">activationCodeCount</span></span>|<span data-ttu-id="a710a-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a710a-153">Int32</span></span>|<span data-ttu-id="a710a-154">Общее количество кодов активации, которые относятся к этому пулу.</span><span class="sxs-lookup"><span data-stu-id="a710a-154">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="a710a-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="a710a-155">Response</span></span>
<span data-ttu-id="a710a-156">В случае успешной работы этот метод возвращает код ответа и встроенный `201 Created` [объектSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a710a-156">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a710a-157">Пример</span><span class="sxs-lookup"><span data-stu-id="a710a-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="a710a-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="a710a-158">Request</span></span>
<span data-ttu-id="a710a-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a710a-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a710a-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="a710a-160">Response</span></span>
<span data-ttu-id="a710a-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a710a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




