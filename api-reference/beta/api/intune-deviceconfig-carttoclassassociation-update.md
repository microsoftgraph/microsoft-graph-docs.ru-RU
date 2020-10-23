---
title: Обновление КарттоклассассоЦиатион
description: Обновление свойств объекта КарттоклассассоЦиатион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc7d72d2d78046654e42007570db26eaaa10102f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722657"
---
# <a name="update-carttoclassassociation"></a><span data-ttu-id="6551e-103">Обновление КарттоклассассоЦиатион</span><span class="sxs-lookup"><span data-stu-id="6551e-103">Update cartToClassAssociation</span></span>

<span data-ttu-id="6551e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6551e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6551e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6551e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6551e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6551e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6551e-107">Обновление свойств объекта [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="6551e-107">Update the properties of a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6551e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6551e-108">Prerequisites</span></span>
<span data-ttu-id="6551e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6551e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6551e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6551e-111">Permission type</span></span>|<span data-ttu-id="6551e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6551e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6551e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6551e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6551e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6551e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6551e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6551e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6551e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6551e-116">Not supported.</span></span>|
|<span data-ttu-id="6551e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6551e-117">Application</span></span>|<span data-ttu-id="6551e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6551e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6551e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6551e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## <a name="request-headers"></a><span data-ttu-id="6551e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6551e-120">Request headers</span></span>
|<span data-ttu-id="6551e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6551e-121">Header</span></span>|<span data-ttu-id="6551e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6551e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6551e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6551e-123">Authorization</span></span>|<span data-ttu-id="6551e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6551e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6551e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6551e-125">Accept</span></span>|<span data-ttu-id="6551e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6551e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6551e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6551e-127">Request body</span></span>
<span data-ttu-id="6551e-128">В тексте запроса добавьте представление объекта [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6551e-128">In the request body, supply a JSON representation for the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

<span data-ttu-id="6551e-129">В следующей таблице приведены свойства, необходимые при создании [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md).</span><span class="sxs-lookup"><span data-stu-id="6551e-129">The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>

|<span data-ttu-id="6551e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6551e-130">Property</span></span>|<span data-ttu-id="6551e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6551e-131">Type</span></span>|<span data-ttu-id="6551e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6551e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6551e-133">id</span><span class="sxs-lookup"><span data-stu-id="6551e-133">id</span></span>|<span data-ttu-id="6551e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6551e-134">String</span></span>|<span data-ttu-id="6551e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6551e-135">Key of the entity.</span></span>|
|<span data-ttu-id="6551e-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6551e-136">createdDateTime</span></span>|<span data-ttu-id="6551e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6551e-137">DateTimeOffset</span></span>|<span data-ttu-id="6551e-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6551e-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="6551e-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6551e-139">lastModifiedDateTime</span></span>|<span data-ttu-id="6551e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6551e-140">DateTimeOffset</span></span>|<span data-ttu-id="6551e-141">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6551e-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="6551e-142">version</span><span class="sxs-lookup"><span data-stu-id="6551e-142">version</span></span>|<span data-ttu-id="6551e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6551e-143">Int32</span></span>|<span data-ttu-id="6551e-144">Версия КарттоклассассоЦиатион.</span><span class="sxs-lookup"><span data-stu-id="6551e-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="6551e-145">displayName</span><span class="sxs-lookup"><span data-stu-id="6551e-145">displayName</span></span>|<span data-ttu-id="6551e-146">Строка</span><span class="sxs-lookup"><span data-stu-id="6551e-146">String</span></span>|<span data-ttu-id="6551e-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6551e-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="6551e-148">description</span><span class="sxs-lookup"><span data-stu-id="6551e-148">description</span></span>|<span data-ttu-id="6551e-149">Строка</span><span class="sxs-lookup"><span data-stu-id="6551e-149">String</span></span>|<span data-ttu-id="6551e-150">Администратор предоставил описание КарттоклассассоЦиатион.</span><span class="sxs-lookup"><span data-stu-id="6551e-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="6551e-151">девицекартидс</span><span class="sxs-lookup"><span data-stu-id="6551e-151">deviceCartIds</span></span>|<span data-ttu-id="6551e-152">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6551e-152">String collection</span></span>|<span data-ttu-id="6551e-153">Идентификаторы корзин устройств, которые необходимо связать с классами.</span><span class="sxs-lookup"><span data-stu-id="6551e-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="6551e-154">классрумидс</span><span class="sxs-lookup"><span data-stu-id="6551e-154">classroomIds</span></span>|<span data-ttu-id="6551e-155">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6551e-155">String collection</span></span>|<span data-ttu-id="6551e-156">Идентификаторы аудиторий, которые необходимо связать с тележками устройств.</span><span class="sxs-lookup"><span data-stu-id="6551e-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="6551e-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="6551e-157">Response</span></span>
<span data-ttu-id="6551e-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6551e-158">If successful, this method returns a `200 OK` response code and an updated [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6551e-159">Пример</span><span class="sxs-lookup"><span data-stu-id="6551e-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="6551e-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="6551e-160">Request</span></span>
<span data-ttu-id="6551e-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6551e-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
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

### <a name="response"></a><span data-ttu-id="6551e-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="6551e-162">Response</span></span>
<span data-ttu-id="6551e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6551e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





