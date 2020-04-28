---
title: Создание КарттоклассассоЦиатион
description: Создание нового объекта КарттоклассассоЦиатион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a694dff31579279e2fd5127157ad4e40786a6f2a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43434418"
---
# <a name="create-carttoclassassociation"></a><span data-ttu-id="8d5b7-103">Создание КарттоклассассоЦиатион</span><span class="sxs-lookup"><span data-stu-id="8d5b7-103">Create cartToClassAssociation</span></span>

<span data-ttu-id="8d5b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d5b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d5b7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d5b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d5b7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d5b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d5b7-107">Создание нового объекта [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="8d5b7-107">Create a new [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d5b7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8d5b7-108">Prerequisites</span></span>
<span data-ttu-id="8d5b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d5b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d5b7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d5b7-111">Permission type</span></span>|<span data-ttu-id="8d5b7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d5b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d5b7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d5b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d5b7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d5b7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d5b7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d5b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d5b7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d5b7-116">Not supported.</span></span>|
|<span data-ttu-id="8d5b7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d5b7-117">Application</span></span>|<span data-ttu-id="8d5b7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d5b7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d5b7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d5b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/cartToClassAssociations
```

## <a name="request-headers"></a><span data-ttu-id="8d5b7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8d5b7-120">Request headers</span></span>
|<span data-ttu-id="8d5b7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d5b7-121">Header</span></span>|<span data-ttu-id="8d5b7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8d5b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d5b7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d5b7-123">Authorization</span></span>|<span data-ttu-id="8d5b7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d5b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d5b7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8d5b7-125">Accept</span></span>|<span data-ttu-id="8d5b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d5b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d5b7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8d5b7-127">Request body</span></span>
<span data-ttu-id="8d5b7-128">В тексте запроса добавьте представление объекта КарттоклассассоЦиатион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d5b7-128">In the request body, supply a JSON representation for the cartToClassAssociation object.</span></span>

<span data-ttu-id="8d5b7-129">В следующей таблице приведены свойства, необходимые при создании КарттоклассассоЦиатион.</span><span class="sxs-lookup"><span data-stu-id="8d5b7-129">The following table shows the properties that are required when you create the cartToClassAssociation.</span></span>

|<span data-ttu-id="8d5b7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d5b7-130">Property</span></span>|<span data-ttu-id="8d5b7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8d5b7-131">Type</span></span>|<span data-ttu-id="8d5b7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8d5b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d5b7-133">id</span><span class="sxs-lookup"><span data-stu-id="8d5b7-133">id</span></span>|<span data-ttu-id="8d5b7-134">String</span><span class="sxs-lookup"><span data-stu-id="8d5b7-134">String</span></span>|<span data-ttu-id="8d5b7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8d5b7-135">Key of the entity.</span></span>|
|<span data-ttu-id="8d5b7-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d5b7-136">createdDateTime</span></span>|<span data-ttu-id="8d5b7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d5b7-137">DateTimeOffset</span></span>|<span data-ttu-id="8d5b7-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8d5b7-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="8d5b7-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d5b7-139">lastModifiedDateTime</span></span>|<span data-ttu-id="8d5b7-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d5b7-140">DateTimeOffset</span></span>|<span data-ttu-id="8d5b7-141">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8d5b7-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="8d5b7-142">version</span><span class="sxs-lookup"><span data-stu-id="8d5b7-142">version</span></span>|<span data-ttu-id="8d5b7-143">Int32</span><span class="sxs-lookup"><span data-stu-id="8d5b7-143">Int32</span></span>|<span data-ttu-id="8d5b7-144">Версия КарттоклассассоЦиатион.</span><span class="sxs-lookup"><span data-stu-id="8d5b7-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="8d5b7-145">displayName</span><span class="sxs-lookup"><span data-stu-id="8d5b7-145">displayName</span></span>|<span data-ttu-id="8d5b7-146">Строка</span><span class="sxs-lookup"><span data-stu-id="8d5b7-146">String</span></span>|<span data-ttu-id="8d5b7-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8d5b7-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="8d5b7-148">description</span><span class="sxs-lookup"><span data-stu-id="8d5b7-148">description</span></span>|<span data-ttu-id="8d5b7-149">String</span><span class="sxs-lookup"><span data-stu-id="8d5b7-149">String</span></span>|<span data-ttu-id="8d5b7-150">Администратор предоставил описание КарттоклассассоЦиатион.</span><span class="sxs-lookup"><span data-stu-id="8d5b7-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="8d5b7-151">девицекартидс</span><span class="sxs-lookup"><span data-stu-id="8d5b7-151">deviceCartIds</span></span>|<span data-ttu-id="8d5b7-152">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="8d5b7-152">String collection</span></span>|<span data-ttu-id="8d5b7-153">Идентификаторы корзин устройств, которые необходимо связать с классами.</span><span class="sxs-lookup"><span data-stu-id="8d5b7-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="8d5b7-154">классрумидс</span><span class="sxs-lookup"><span data-stu-id="8d5b7-154">classroomIds</span></span>|<span data-ttu-id="8d5b7-155">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="8d5b7-155">String collection</span></span>|<span data-ttu-id="8d5b7-156">Идентификаторы аудиторий, которые необходимо связать с тележками устройств.</span><span class="sxs-lookup"><span data-stu-id="8d5b7-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="8d5b7-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d5b7-157">Response</span></span>
<span data-ttu-id="8d5b7-158">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8d5b7-158">If successful, this method returns a `201 Created` response code and a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d5b7-159">Пример</span><span class="sxs-lookup"><span data-stu-id="8d5b7-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d5b7-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d5b7-160">Request</span></span>
<span data-ttu-id="8d5b7-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d5b7-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8d5b7-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d5b7-162">Response</span></span>
<span data-ttu-id="8d5b7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d5b7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



