---
title: Тип ресурса договора
description: Представляет настраиваемое соглашение об использовании клиента, которое создается и управляется с помощью Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: b6b3ca4865e56961f6388e9be1a567de73026472
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643997"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="1d88e-103">Тип ресурса договора</span><span class="sxs-lookup"><span data-stu-id="1d88e-103">agreement resource type</span></span>

<span data-ttu-id="1d88e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d88e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d88e-105">Представляет настраиваемое соглашение об использовании клиента, которое создается и управляется с помощью Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="1d88e-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="1d88e-106">Вы можете использовать следующие методы для создания и управления [условиями использования функции Azure Active Directory](/azure/active-directory/active-directory-tou) в соответствии со сценарием.</span><span class="sxs-lookup"><span data-stu-id="1d88e-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="1d88e-107">Методы</span><span class="sxs-lookup"><span data-stu-id="1d88e-107">Methods</span></span>

| <span data-ttu-id="1d88e-108">Метод</span><span class="sxs-lookup"><span data-stu-id="1d88e-108">Method</span></span>       | <span data-ttu-id="1d88e-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1d88e-109">Return Type</span></span> | <span data-ttu-id="1d88e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1d88e-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1d88e-111">Создание договоров</span><span class="sxs-lookup"><span data-stu-id="1d88e-111">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="1d88e-112">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="1d88e-112">agreement</span></span>](agreement.md) | <span data-ttu-id="1d88e-113">Создание нового соглашения путем публикации в коллекции договоров.</span><span class="sxs-lookup"><span data-stu-id="1d88e-113">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="1d88e-114">Список соглашений</span><span class="sxs-lookup"><span data-stu-id="1d88e-114">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="1d88e-115">Коллекция [договоров](agreement.md)</span><span class="sxs-lookup"><span data-stu-id="1d88e-115">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="1d88e-116">Получение коллекции объектов Agreement.</span><span class="sxs-lookup"><span data-stu-id="1d88e-116">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="1d88e-117">Получение соглашения</span><span class="sxs-lookup"><span data-stu-id="1d88e-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="1d88e-118">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="1d88e-118">agreement</span></span>](agreement.md) | <span data-ttu-id="1d88e-119">Чтение свойств и связей объекта Agreement.</span><span class="sxs-lookup"><span data-stu-id="1d88e-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="1d88e-120">Обновление соглашения</span><span class="sxs-lookup"><span data-stu-id="1d88e-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="1d88e-121">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="1d88e-121">agreement</span></span>](agreement.md) | <span data-ttu-id="1d88e-122">Обновление объекта договора.</span><span class="sxs-lookup"><span data-stu-id="1d88e-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="1d88e-123">Удаление соглашения</span><span class="sxs-lookup"><span data-stu-id="1d88e-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="1d88e-124">Нет</span><span class="sxs-lookup"><span data-stu-id="1d88e-124">None</span></span> | <span data-ttu-id="1d88e-125">Удаление объекта соглашения.</span><span class="sxs-lookup"><span data-stu-id="1d88e-125">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="1d88e-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d88e-126">Properties</span></span>
| <span data-ttu-id="1d88e-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d88e-127">Property</span></span>     | <span data-ttu-id="1d88e-128">Тип</span><span class="sxs-lookup"><span data-stu-id="1d88e-128">Type</span></span>        | <span data-ttu-id="1d88e-129">Описание</span><span class="sxs-lookup"><span data-stu-id="1d88e-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1d88e-130">displayName</span><span class="sxs-lookup"><span data-stu-id="1d88e-130">displayName</span></span>|<span data-ttu-id="1d88e-131">String</span><span class="sxs-lookup"><span data-stu-id="1d88e-131">String</span></span>|<span data-ttu-id="1d88e-132">Отображаемое имя соглашения.</span><span class="sxs-lookup"><span data-stu-id="1d88e-132">Display name of the agreement.</span></span> <span data-ttu-id="1d88e-133">Отображаемое имя используется для внутренней трассировки соглашения, но оно не отображается для конечных пользователей, которые просматривают соглашение.</span><span class="sxs-lookup"><span data-stu-id="1d88e-133">The display name is used for internal tracking of the agreement but is not shown to end users who view the agreement.</span></span>|
|<span data-ttu-id="1d88e-134">id</span><span class="sxs-lookup"><span data-stu-id="1d88e-134">id</span></span>|<span data-ttu-id="1d88e-135">String</span><span class="sxs-lookup"><span data-stu-id="1d88e-135">String</span></span>| <span data-ttu-id="1d88e-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d88e-136">Read-only.</span></span>|
|<span data-ttu-id="1d88e-137">испердевицеакцептанцерекуиред</span><span class="sxs-lookup"><span data-stu-id="1d88e-137">isPerDeviceAcceptanceRequired</span></span>|<span data-ttu-id="1d88e-138">Логический</span><span class="sxs-lookup"><span data-stu-id="1d88e-138">Boolean</span></span>|<span data-ttu-id="1d88e-139">Этот параметр позволяет конечным пользователям принимать данное соглашение для всех устройств, к которым они обращаются.</span><span class="sxs-lookup"><span data-stu-id="1d88e-139">This setting enables you to require end users to accept this agreement on every device that they are accessing it from.</span></span> <span data-ttu-id="1d88e-140">Конечному пользователю потребуется зарегистрировать свое устройство в Azure AD, если это еще не сделано.</span><span class="sxs-lookup"><span data-stu-id="1d88e-140">The end user will be required to register their device in Azure AD, if they haven't already done so.</span></span>|
|<span data-ttu-id="1d88e-141">исвиевингбефореакцептанцерекуиред</span><span class="sxs-lookup"><span data-stu-id="1d88e-141">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="1d88e-142">Логический</span><span class="sxs-lookup"><span data-stu-id="1d88e-142">Boolean</span></span>|<span data-ttu-id="1d88e-143">Указывает, должно ли пользователь расширить Соглашение перед принятием.</span><span class="sxs-lookup"><span data-stu-id="1d88e-143">Indicates whether the user has to expand the agreement before accepting.</span></span>|
|<span data-ttu-id="1d88e-144">термсекспиратион</span><span class="sxs-lookup"><span data-stu-id="1d88e-144">termsExpiration</span></span>|[<span data-ttu-id="1d88e-145">термсекспиратион</span><span class="sxs-lookup"><span data-stu-id="1d88e-145">termsExpiration</span></span>](termsexpiration.md)| <span data-ttu-id="1d88e-146">Расписание истечения срока действия и периодичность соглашения для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="1d88e-146">Expiration schedule and frequency of agreement for all users.</span></span> |
|<span data-ttu-id="1d88e-147">усерреакцептрекуиредфрекуенци</span><span class="sxs-lookup"><span data-stu-id="1d88e-147">userReacceptRequiredFrequency</span></span>|<span data-ttu-id="1d88e-148">Длительность</span><span class="sxs-lookup"><span data-stu-id="1d88e-148">Duration</span></span>|<span data-ttu-id="1d88e-149">Срок действия, по истечении которого пользователь должен повторно принять условия использования.</span><span class="sxs-lookup"><span data-stu-id="1d88e-149">The duration after which the user must re-accept the terms of use.</span></span> <span data-ttu-id="1d88e-150">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="1d88e-150">The value is represented in ISO 8601 format for durations.</span></span>|


## <a name="relationships"></a><span data-ttu-id="1d88e-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="1d88e-151">Relationships</span></span>
| <span data-ttu-id="1d88e-152">Связь</span><span class="sxs-lookup"><span data-stu-id="1d88e-152">Relationship</span></span> | <span data-ttu-id="1d88e-153">Тип</span><span class="sxs-lookup"><span data-stu-id="1d88e-153">Type</span></span>        | <span data-ttu-id="1d88e-154">Описание</span><span class="sxs-lookup"><span data-stu-id="1d88e-154">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1d88e-155">приемы</span><span class="sxs-lookup"><span data-stu-id="1d88e-155">acceptances</span></span>|<span data-ttu-id="1d88e-156">Коллекция [agreementAcceptance](agreementacceptance.md)</span><span class="sxs-lookup"><span data-stu-id="1d88e-156">[agreementAcceptance](agreementacceptance.md) collection</span></span>|<span data-ttu-id="1d88e-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d88e-157">Read-only.</span></span> <span data-ttu-id="1d88e-158">Сведения о приемках настоящего соглашения.</span><span class="sxs-lookup"><span data-stu-id="1d88e-158">Information about acceptances of this agreement.</span></span>|
|<span data-ttu-id="1d88e-159">files</span><span class="sxs-lookup"><span data-stu-id="1d88e-159">files</span></span>|<span data-ttu-id="1d88e-160">Коллекция [агриментфилелокализатион](agreementfilelocalization.md)</span><span class="sxs-lookup"><span data-stu-id="1d88e-160">[agreementFileLocalization](agreementfilelocalization.md) collection</span></span>| <span data-ttu-id="1d88e-161">Документы PDF, связанные с этим соглашением.</span><span class="sxs-lookup"><span data-stu-id="1d88e-161">PDFs linked to this agreement.</span></span> <span data-ttu-id="1d88e-162">**Примечание:** Это свойство является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="1d88e-162">**Note:** This property is in the process of being deprecated.</span></span> <span data-ttu-id="1d88e-163">Вместо этого свойству **файла** усесе.</span><span class="sxs-lookup"><span data-stu-id="1d88e-163">Usethe  **file** property instead.</span></span>|
|<span data-ttu-id="1d88e-164">file</span><span class="sxs-lookup"><span data-stu-id="1d88e-164">file</span></span>|[<span data-ttu-id="1d88e-165">агриментфиле</span><span class="sxs-lookup"><span data-stu-id="1d88e-165">agreementFile</span></span>](agreementfile.md) | <span data-ttu-id="1d88e-166">Документы PDF, связанные с этим соглашением.</span><span class="sxs-lookup"><span data-stu-id="1d88e-166">PDFs linked to this agreement.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1d88e-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d88e-167">JSON representation</span></span>

<span data-ttu-id="1d88e-168">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d88e-168">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreement"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "isPerDeviceAcceptanceRequired": false,
  "termsExpiration": {
    "startDateTime": "2018-10-01T00:00:00.0000000Z",
    "frequency": "PT1M"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
