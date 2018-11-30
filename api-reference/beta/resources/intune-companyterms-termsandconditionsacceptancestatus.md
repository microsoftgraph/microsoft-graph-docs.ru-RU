---
title: Тип ресурса termsAndConditionsAcceptanceStatus
description: C) политики данным пользователем. Чтобы получить доступ к корпоративному порталу, пользователям нужно принять последнюю версию условий.
ms.openlocfilehash: a1cb2d53a0ebb2cb42868ba0041a59fc22992575
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079638"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="fa840-104">Тип ресурса termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="fa840-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="fa840-105">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fa840-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa840-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa840-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa840-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fa840-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa840-108">Объект termsAndConditionsAcceptanceStatus представляет состояние принятия определенной политики условий для заданного пользователя.</span><span class="sxs-lookup"><span data-stu-id="fa840-108">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="fa840-109">Чтобы получить доступ к корпоративному порталу, пользователям нужно принять последнюю версию условий.</span><span class="sxs-lookup"><span data-stu-id="fa840-109">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>
## <a name="methods"></a><span data-ttu-id="fa840-110">Методы</span><span class="sxs-lookup"><span data-stu-id="fa840-110">Methods</span></span>
|<span data-ttu-id="fa840-111">Метод</span><span class="sxs-lookup"><span data-stu-id="fa840-111">Method</span></span>|<span data-ttu-id="fa840-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fa840-112">Return Type</span></span>|<span data-ttu-id="fa840-113">Описание</span><span class="sxs-lookup"><span data-stu-id="fa840-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fa840-114">Список termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="fa840-114">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="fa840-115">Коллекция [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)</span><span class="sxs-lookup"><span data-stu-id="fa840-115">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="fa840-116">Список свойств и связей объектов [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="fa840-116">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="fa840-117">Получение объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="fa840-117">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="fa840-118">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="fa840-118">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="fa840-119">Чтение свойств и связей объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="fa840-119">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="fa840-120">Создание объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="fa840-120">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="fa840-121">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="fa840-121">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="fa840-122">Создание объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="fa840-122">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="fa840-123">Удаление объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="fa840-123">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="fa840-124">Нет</span><span class="sxs-lookup"><span data-stu-id="fa840-124">None</span></span>|<span data-ttu-id="fa840-125">Удаляет объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="fa840-125">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="fa840-126">Обновление объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="fa840-126">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="fa840-127">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="fa840-127">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="fa840-128">Обновление свойств объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="fa840-128">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fa840-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa840-129">Properties</span></span>
|<span data-ttu-id="fa840-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa840-130">Property</span></span>|<span data-ttu-id="fa840-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fa840-131">Type</span></span>|<span data-ttu-id="fa840-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fa840-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa840-133">id</span><span class="sxs-lookup"><span data-stu-id="fa840-133">id</span></span>|<span data-ttu-id="fa840-134">String</span><span class="sxs-lookup"><span data-stu-id="fa840-134">String</span></span>|<span data-ttu-id="fa840-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="fa840-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="fa840-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="fa840-136">userDisplayName</span></span>|<span data-ttu-id="fa840-137">String</span><span class="sxs-lookup"><span data-stu-id="fa840-137">String</span></span>|<span data-ttu-id="fa840-138">Отображает имя пользователя, чье принятие представлено объектом.</span><span class="sxs-lookup"><span data-stu-id="fa840-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="fa840-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="fa840-139">acceptedVersion</span></span>|<span data-ttu-id="fa840-140">Int32</span><span class="sxs-lookup"><span data-stu-id="fa840-140">Int32</span></span>|<span data-ttu-id="fa840-141">Номер последней версии условий, принятых пользователем.</span><span class="sxs-lookup"><span data-stu-id="fa840-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="fa840-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa840-142">acceptedDateTime</span></span>|<span data-ttu-id="fa840-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa840-143">DateTimeOffset</span></span>|<span data-ttu-id="fa840-144">Дата и время последнего принятия условий пользователем.</span><span class="sxs-lookup"><span data-stu-id="fa840-144">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa840-145">Связи</span><span class="sxs-lookup"><span data-stu-id="fa840-145">Relationships</span></span>
|<span data-ttu-id="fa840-146">Связь</span><span class="sxs-lookup"><span data-stu-id="fa840-146">Relationship</span></span>|<span data-ttu-id="fa840-147">Тип</span><span class="sxs-lookup"><span data-stu-id="fa840-147">Type</span></span>|<span data-ttu-id="fa840-148">Описание</span><span class="sxs-lookup"><span data-stu-id="fa840-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa840-149">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="fa840-149">termsAndConditions</span></span>|[<span data-ttu-id="fa840-150">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="fa840-150">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="fa840-151">Ссылка для перехода к назначенным условиям.</span><span class="sxs-lookup"><span data-stu-id="fa840-151">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa840-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa840-152">JSON Representation</span></span>
<span data-ttu-id="fa840-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa840-153">Here is a JSON representation of the resource.</span></span>
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





