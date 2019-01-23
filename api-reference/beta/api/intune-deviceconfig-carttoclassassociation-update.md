---
title: Обновление cartToClassAssociation
description: Обновление свойства объекта cartToClassAssociation.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a8da37fa694c0352ade04c1ae9ce9bca926bc126
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396800"
---
# <a name="update-carttoclassassociation"></a><span data-ttu-id="bc32b-103">Обновление cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="bc32b-103">Update cartToClassAssociation</span></span>

> <span data-ttu-id="bc32b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bc32b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bc32b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc32b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc32b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc32b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc32b-107">Обновление свойства объекта [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="bc32b-107">Update the properties of a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc32b-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="bc32b-108">Prerequisites</span></span>
<span data-ttu-id="bc32b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bc32b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bc32b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc32b-111">Permission type</span></span>|<span data-ttu-id="bc32b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc32b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc32b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc32b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc32b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc32b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc32b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc32b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc32b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc32b-116">Not supported.</span></span>|
|<span data-ttu-id="bc32b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc32b-117">Application</span></span>|<span data-ttu-id="bc32b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc32b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc32b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc32b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## <a name="request-headers"></a><span data-ttu-id="bc32b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc32b-120">Request headers</span></span>
|<span data-ttu-id="bc32b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc32b-121">Header</span></span>|<span data-ttu-id="bc32b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bc32b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc32b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc32b-123">Authorization</span></span>|<span data-ttu-id="bc32b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bc32b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc32b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bc32b-125">Accept</span></span>|<span data-ttu-id="bc32b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc32b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc32b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc32b-127">Request body</span></span>
<span data-ttu-id="bc32b-128">В тексте запроса укажите представление JSON для объекта [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="bc32b-128">In the request body, supply a JSON representation for the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

<span data-ttu-id="bc32b-129">В следующей таблице показаны свойства, которые необходимы для создания [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span><span class="sxs-lookup"><span data-stu-id="bc32b-129">The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>

|<span data-ttu-id="bc32b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc32b-130">Property</span></span>|<span data-ttu-id="bc32b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bc32b-131">Type</span></span>|<span data-ttu-id="bc32b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bc32b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc32b-133">id</span><span class="sxs-lookup"><span data-stu-id="bc32b-133">id</span></span>|<span data-ttu-id="bc32b-134">String</span><span class="sxs-lookup"><span data-stu-id="bc32b-134">String</span></span>|<span data-ttu-id="bc32b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bc32b-135">Key of the entity.</span></span>|
|<span data-ttu-id="bc32b-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc32b-136">createdDateTime</span></span>|<span data-ttu-id="bc32b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc32b-137">DateTimeOffset</span></span>|<span data-ttu-id="bc32b-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bc32b-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="bc32b-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc32b-139">lastModifiedDateTime</span></span>|<span data-ttu-id="bc32b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc32b-140">DateTimeOffset</span></span>|<span data-ttu-id="bc32b-141">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bc32b-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="bc32b-142">version</span><span class="sxs-lookup"><span data-stu-id="bc32b-142">version</span></span>|<span data-ttu-id="bc32b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="bc32b-143">Int32</span></span>|<span data-ttu-id="bc32b-144">Версия CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="bc32b-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="bc32b-145">displayName</span><span class="sxs-lookup"><span data-stu-id="bc32b-145">displayName</span></span>|<span data-ttu-id="bc32b-146">String</span><span class="sxs-lookup"><span data-stu-id="bc32b-146">String</span></span>|<span data-ttu-id="bc32b-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bc32b-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="bc32b-148">description</span><span class="sxs-lookup"><span data-stu-id="bc32b-148">description</span></span>|<span data-ttu-id="bc32b-149">String</span><span class="sxs-lookup"><span data-stu-id="bc32b-149">String</span></span>|<span data-ttu-id="bc32b-150">Admin, предоставляемые описание CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="bc32b-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="bc32b-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="bc32b-151">deviceCartIds</span></span>|<span data-ttu-id="bc32b-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bc32b-152">String collection</span></span>|<span data-ttu-id="bc32b-153">Идентификаторы корзины устройства необходимо сопоставить с классы.</span><span class="sxs-lookup"><span data-stu-id="bc32b-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="bc32b-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="bc32b-154">classroomIds</span></span>|<span data-ttu-id="bc32b-155">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bc32b-155">String collection</span></span>|<span data-ttu-id="bc32b-156">Идентификаторы аудиторий необходимо сопоставить с устройства корзины.</span><span class="sxs-lookup"><span data-stu-id="bc32b-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="bc32b-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc32b-157">Response</span></span>
<span data-ttu-id="bc32b-158">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bc32b-158">If successful, this method returns a `200 OK` response code and an updated [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc32b-159">Пример</span><span class="sxs-lookup"><span data-stu-id="bc32b-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc32b-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc32b-160">Request</span></span>
<span data-ttu-id="bc32b-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc32b-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bc32b-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc32b-162">Response</span></span>
<span data-ttu-id="bc32b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bc32b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




