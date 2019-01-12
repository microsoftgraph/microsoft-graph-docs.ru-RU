---
title: Тип ресурса termsAndConditionsAcceptanceStatus
description: C) политики данным пользователем. Чтобы получить доступ к корпоративному порталу, пользователям нужно принять последнюю версию условий.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dffbcf3b13fd988a75e4f1061a52dfc46f193bb5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971377"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="8fef3-104">Тип ресурса termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="8fef3-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="8fef3-105">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8fef3-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8fef3-106">Объект termsAndConditionsAcceptanceStatus представляет состояние принятия определенной политики условий для заданного пользователя.</span><span class="sxs-lookup"><span data-stu-id="8fef3-106">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="8fef3-107">Чтобы получить доступ к корпоративному порталу, пользователям нужно принять последнюю версию условий.</span><span class="sxs-lookup"><span data-stu-id="8fef3-107">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>
## <a name="methods"></a><span data-ttu-id="8fef3-108">Методы</span><span class="sxs-lookup"><span data-stu-id="8fef3-108">Methods</span></span>
|<span data-ttu-id="8fef3-109">Метод</span><span class="sxs-lookup"><span data-stu-id="8fef3-109">Method</span></span>|<span data-ttu-id="8fef3-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8fef3-110">Return Type</span></span>|<span data-ttu-id="8fef3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8fef3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8fef3-112">Список termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="8fef3-112">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="8fef3-113">Коллекция [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)</span><span class="sxs-lookup"><span data-stu-id="8fef3-113">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="8fef3-114">Список свойств и связей объектов [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8fef3-114">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="8fef3-115">Получение объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="8fef3-115">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="8fef3-116">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="8fef3-116">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="8fef3-117">Чтение свойств и связей объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8fef3-117">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="8fef3-118">Создание объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="8fef3-118">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="8fef3-119">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="8fef3-119">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="8fef3-120">Создание объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8fef3-120">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="8fef3-121">Удаление объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="8fef3-121">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="8fef3-122">Нет</span><span class="sxs-lookup"><span data-stu-id="8fef3-122">None</span></span>|<span data-ttu-id="8fef3-123">Удаляет объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8fef3-123">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="8fef3-124">Обновление объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="8fef3-124">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="8fef3-125">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="8fef3-125">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="8fef3-126">Обновление свойств объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8fef3-126">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8fef3-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="8fef3-127">Properties</span></span>
|<span data-ttu-id="8fef3-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="8fef3-128">Property</span></span>|<span data-ttu-id="8fef3-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8fef3-129">Type</span></span>|<span data-ttu-id="8fef3-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8fef3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fef3-131">id</span><span class="sxs-lookup"><span data-stu-id="8fef3-131">id</span></span>|<span data-ttu-id="8fef3-132">String</span><span class="sxs-lookup"><span data-stu-id="8fef3-132">String</span></span>|<span data-ttu-id="8fef3-133">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="8fef3-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="8fef3-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="8fef3-134">userDisplayName</span></span>|<span data-ttu-id="8fef3-135">String</span><span class="sxs-lookup"><span data-stu-id="8fef3-135">String</span></span>|<span data-ttu-id="8fef3-136">Отображает имя пользователя, чье принятие представлено объектом.</span><span class="sxs-lookup"><span data-stu-id="8fef3-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="8fef3-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="8fef3-137">acceptedVersion</span></span>|<span data-ttu-id="8fef3-138">Int32</span><span class="sxs-lookup"><span data-stu-id="8fef3-138">Int32</span></span>|<span data-ttu-id="8fef3-139">Номер последней версии условий, принятых пользователем.</span><span class="sxs-lookup"><span data-stu-id="8fef3-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="8fef3-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="8fef3-140">acceptedDateTime</span></span>|<span data-ttu-id="8fef3-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fef3-141">DateTimeOffset</span></span>|<span data-ttu-id="8fef3-142">Дата и время последнего принятия условий пользователем.</span><span class="sxs-lookup"><span data-stu-id="8fef3-142">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fef3-143">Связи</span><span class="sxs-lookup"><span data-stu-id="8fef3-143">Relationships</span></span>
|<span data-ttu-id="8fef3-144">Связь</span><span class="sxs-lookup"><span data-stu-id="8fef3-144">Relationship</span></span>|<span data-ttu-id="8fef3-145">Тип</span><span class="sxs-lookup"><span data-stu-id="8fef3-145">Type</span></span>|<span data-ttu-id="8fef3-146">Описание</span><span class="sxs-lookup"><span data-stu-id="8fef3-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fef3-147">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="8fef3-147">termsAndConditions</span></span>|[<span data-ttu-id="8fef3-148">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="8fef3-148">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="8fef3-149">Ссылка для перехода к назначенным условиям.</span><span class="sxs-lookup"><span data-stu-id="8fef3-149">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8fef3-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8fef3-150">JSON Representation</span></span>
<span data-ttu-id="8fef3-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8fef3-151">Here is a JSON representation of the resource.</span></span>
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



