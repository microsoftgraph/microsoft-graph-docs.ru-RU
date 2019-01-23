---
title: Тип ресурса termsAndConditionsAcceptanceStatus
description: Объект termsAndConditionsAcceptanceStatus представляет состояние принятия определенной политики условий для заданного пользователя. Чтобы получить доступ к корпоративному порталу, пользователям нужно принять последнюю версию условий.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e6156c1f5cf952f485e6f0a210a7aef4bd7b3ac
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412557"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="9cca5-104">Тип ресурса termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="9cca5-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="9cca5-105">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9cca5-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9cca5-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cca5-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9cca5-107">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9cca5-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cca5-108">Объект termsAndConditionsAcceptanceStatus представляет состояние принятия определенной политики условий для заданного пользователя.</span><span class="sxs-lookup"><span data-stu-id="9cca5-108">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="9cca5-109">Чтобы получить доступ к корпоративному порталу, пользователям нужно принять последнюю версию условий.</span><span class="sxs-lookup"><span data-stu-id="9cca5-109">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>

## <a name="methods"></a><span data-ttu-id="9cca5-110">Методы</span><span class="sxs-lookup"><span data-stu-id="9cca5-110">Methods</span></span>
|<span data-ttu-id="9cca5-111">Метод</span><span class="sxs-lookup"><span data-stu-id="9cca5-111">Method</span></span>|<span data-ttu-id="9cca5-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9cca5-112">Return Type</span></span>|<span data-ttu-id="9cca5-113">Описание</span><span class="sxs-lookup"><span data-stu-id="9cca5-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9cca5-114">Список termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="9cca5-114">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="9cca5-115">Коллекция [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)</span><span class="sxs-lookup"><span data-stu-id="9cca5-115">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="9cca5-116">Список свойств и связей объектов [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="9cca5-116">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="9cca5-117">Получение объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="9cca5-117">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="9cca5-118">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="9cca5-118">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="9cca5-119">Чтение свойств и связей объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="9cca5-119">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="9cca5-120">Создание объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="9cca5-120">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="9cca5-121">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="9cca5-121">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="9cca5-122">Создание объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="9cca5-122">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="9cca5-123">Удаление объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="9cca5-123">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="9cca5-124">Нет</span><span class="sxs-lookup"><span data-stu-id="9cca5-124">None</span></span>|<span data-ttu-id="9cca5-125">Удаляет объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="9cca5-125">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="9cca5-126">Обновление объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="9cca5-126">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="9cca5-127">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="9cca5-127">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="9cca5-128">Обновление свойств объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="9cca5-128">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9cca5-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="9cca5-129">Properties</span></span>
|<span data-ttu-id="9cca5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9cca5-130">Property</span></span>|<span data-ttu-id="9cca5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9cca5-131">Type</span></span>|<span data-ttu-id="9cca5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9cca5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cca5-133">id</span><span class="sxs-lookup"><span data-stu-id="9cca5-133">id</span></span>|<span data-ttu-id="9cca5-134">String</span><span class="sxs-lookup"><span data-stu-id="9cca5-134">String</span></span>|<span data-ttu-id="9cca5-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="9cca5-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="9cca5-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="9cca5-136">userDisplayName</span></span>|<span data-ttu-id="9cca5-137">String</span><span class="sxs-lookup"><span data-stu-id="9cca5-137">String</span></span>|<span data-ttu-id="9cca5-138">Отображает имя пользователя, чье принятие представлено объектом.</span><span class="sxs-lookup"><span data-stu-id="9cca5-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="9cca5-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="9cca5-139">acceptedVersion</span></span>|<span data-ttu-id="9cca5-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9cca5-140">Int32</span></span>|<span data-ttu-id="9cca5-141">Номер последней версии условий, принятых пользователем.</span><span class="sxs-lookup"><span data-stu-id="9cca5-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="9cca5-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="9cca5-142">acceptedDateTime</span></span>|<span data-ttu-id="9cca5-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cca5-143">DateTimeOffset</span></span>|<span data-ttu-id="9cca5-144">Дата и время последнего принятия условий пользователем.</span><span class="sxs-lookup"><span data-stu-id="9cca5-144">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9cca5-145">Связи</span><span class="sxs-lookup"><span data-stu-id="9cca5-145">Relationships</span></span>
|<span data-ttu-id="9cca5-146">Связь</span><span class="sxs-lookup"><span data-stu-id="9cca5-146">Relationship</span></span>|<span data-ttu-id="9cca5-147">Тип</span><span class="sxs-lookup"><span data-stu-id="9cca5-147">Type</span></span>|<span data-ttu-id="9cca5-148">Описание</span><span class="sxs-lookup"><span data-stu-id="9cca5-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cca5-149">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="9cca5-149">termsAndConditions</span></span>|[<span data-ttu-id="9cca5-150">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="9cca5-150">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="9cca5-151">Ссылка для перехода к назначенным условиям.</span><span class="sxs-lookup"><span data-stu-id="9cca5-151">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9cca5-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9cca5-152">JSON Representation</span></span>
<span data-ttu-id="9cca5-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9cca5-153">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)"
}
```




