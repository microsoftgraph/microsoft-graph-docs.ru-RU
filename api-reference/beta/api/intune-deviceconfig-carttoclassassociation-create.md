---
title: Создание КарттоклассассоЦиатион
description: Создание нового объекта КарттоклассассоЦиатион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2338e879df9f7e1920c90df61dda62a86d1bc2db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443330"
---
# <a name="create-carttoclassassociation"></a><span data-ttu-id="d4379-103">Создание КарттоклассассоЦиатион</span><span class="sxs-lookup"><span data-stu-id="d4379-103">Create cartToClassAssociation</span></span>

<span data-ttu-id="d4379-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d4379-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4379-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4379-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4379-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4379-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4379-107">Создание нового объекта [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="d4379-107">Create a new [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4379-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d4379-108">Prerequisites</span></span>
<span data-ttu-id="d4379-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4379-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4379-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4379-111">Permission type</span></span>|<span data-ttu-id="d4379-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4379-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4379-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4379-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4379-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4379-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4379-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4379-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4379-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4379-116">Not supported.</span></span>|
|<span data-ttu-id="d4379-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4379-117">Application</span></span>|<span data-ttu-id="d4379-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4379-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4379-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4379-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/cartToClassAssociations
```

## <a name="request-headers"></a><span data-ttu-id="d4379-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d4379-120">Request headers</span></span>
|<span data-ttu-id="d4379-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4379-121">Header</span></span>|<span data-ttu-id="d4379-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d4379-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4379-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4379-123">Authorization</span></span>|<span data-ttu-id="d4379-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4379-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4379-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d4379-125">Accept</span></span>|<span data-ttu-id="d4379-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4379-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4379-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4379-127">Request body</span></span>
<span data-ttu-id="d4379-128">В тексте запроса добавьте представление объекта КарттоклассассоЦиатион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4379-128">In the request body, supply a JSON representation for the cartToClassAssociation object.</span></span>

<span data-ttu-id="d4379-129">В следующей таблице приведены свойства, необходимые при создании КарттоклассассоЦиатион.</span><span class="sxs-lookup"><span data-stu-id="d4379-129">The following table shows the properties that are required when you create the cartToClassAssociation.</span></span>

|<span data-ttu-id="d4379-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4379-130">Property</span></span>|<span data-ttu-id="d4379-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d4379-131">Type</span></span>|<span data-ttu-id="d4379-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d4379-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4379-133">id</span><span class="sxs-lookup"><span data-stu-id="d4379-133">id</span></span>|<span data-ttu-id="d4379-134">String</span><span class="sxs-lookup"><span data-stu-id="d4379-134">String</span></span>|<span data-ttu-id="d4379-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d4379-135">Key of the entity.</span></span>|
|<span data-ttu-id="d4379-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4379-136">createdDateTime</span></span>|<span data-ttu-id="d4379-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4379-137">DateTimeOffset</span></span>|<span data-ttu-id="d4379-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d4379-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="d4379-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4379-139">lastModifiedDateTime</span></span>|<span data-ttu-id="d4379-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4379-140">DateTimeOffset</span></span>|<span data-ttu-id="d4379-141">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d4379-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="d4379-142">version</span><span class="sxs-lookup"><span data-stu-id="d4379-142">version</span></span>|<span data-ttu-id="d4379-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d4379-143">Int32</span></span>|<span data-ttu-id="d4379-144">Версия КарттоклассассоЦиатион.</span><span class="sxs-lookup"><span data-stu-id="d4379-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="d4379-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d4379-145">displayName</span></span>|<span data-ttu-id="d4379-146">Строка</span><span class="sxs-lookup"><span data-stu-id="d4379-146">String</span></span>|<span data-ttu-id="d4379-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d4379-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="d4379-148">description</span><span class="sxs-lookup"><span data-stu-id="d4379-148">description</span></span>|<span data-ttu-id="d4379-149">String</span><span class="sxs-lookup"><span data-stu-id="d4379-149">String</span></span>|<span data-ttu-id="d4379-150">Администратор предоставил описание КарттоклассассоЦиатион.</span><span class="sxs-lookup"><span data-stu-id="d4379-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="d4379-151">девицекартидс</span><span class="sxs-lookup"><span data-stu-id="d4379-151">deviceCartIds</span></span>|<span data-ttu-id="d4379-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d4379-152">String collection</span></span>|<span data-ttu-id="d4379-153">Идентификаторы корзин устройств, которые необходимо связать с классами.</span><span class="sxs-lookup"><span data-stu-id="d4379-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="d4379-154">классрумидс</span><span class="sxs-lookup"><span data-stu-id="d4379-154">classroomIds</span></span>|<span data-ttu-id="d4379-155">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d4379-155">String collection</span></span>|<span data-ttu-id="d4379-156">Идентификаторы аудиторий, которые необходимо связать с тележками устройств.</span><span class="sxs-lookup"><span data-stu-id="d4379-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="d4379-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4379-157">Response</span></span>
<span data-ttu-id="d4379-158">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4379-158">If successful, this method returns a `201 Created` response code and a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4379-159">Пример</span><span class="sxs-lookup"><span data-stu-id="d4379-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4379-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4379-160">Request</span></span>
<span data-ttu-id="d4379-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4379-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="d4379-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4379-162">Response</span></span>
<span data-ttu-id="d4379-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4379-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "9bdc58dd-58dd-9bdc-dd58-dc9bdd58dc9b",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```





