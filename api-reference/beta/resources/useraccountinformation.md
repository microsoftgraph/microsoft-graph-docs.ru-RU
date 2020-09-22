---
title: Тип ресурса Усераккаунтинформатион
description: Тип ресурса Усераккаунтинформатион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 9bcd0553c51d75724f28737321f463bcab034306
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057915"
---
# <a name="useraccountinformation-resource-type"></a><span data-ttu-id="46714-103">Тип ресурса Усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="46714-103">userAccountInformation resource type</span></span>

<span data-ttu-id="46714-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46714-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46714-105">Представляет сведения, специально связанные с учетной записью пользователя, будь то учетная запись Azure AD или учетная запись Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="46714-105">Represents information specifically tied to a user's account, whether that is as an Azure AD account or Microsoft account.</span></span> <span data-ttu-id="46714-106">Идентификатор сущности задается соответствующим идентификаторам Azure AD AD или CID учетной записи Майкрософт соответственно.</span><span class="sxs-lookup"><span data-stu-id="46714-106">The entity identifier is set to the corresponding Azure AD guid or Microsoft Account CID respectively.</span></span> <span data-ttu-id="46714-107">Эти поля доступны только для чтения через Microsoft Graph и должны редактироваться с помощью профиля пользователя или администратора клиента для соответствующего интерфейса.</span><span class="sxs-lookup"><span data-stu-id="46714-107">These fields are read-only through Microsoft Graph and must be edited through a users profile or by a Tenant Administrator on a corresponding experience.</span></span>

<span data-ttu-id="46714-108">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="46714-108">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="46714-109">Методы</span><span class="sxs-lookup"><span data-stu-id="46714-109">Methods</span></span>

|<span data-ttu-id="46714-110">Метод</span><span class="sxs-lookup"><span data-stu-id="46714-110">Method</span></span>|<span data-ttu-id="46714-111">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="46714-111">Return type</span></span>|<span data-ttu-id="46714-112">Описание</span><span class="sxs-lookup"><span data-stu-id="46714-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="46714-113">Список учетных записей</span><span class="sxs-lookup"><span data-stu-id="46714-113">List accounts</span></span>](../api/profile-list-accounts.md)|<span data-ttu-id="46714-114">Коллекция [усераккаунтинформатион](../resources/useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="46714-114">[userAccountInformation](../resources/useraccountinformation.md) collection</span></span>|<span data-ttu-id="46714-115">Получение ресурсов Усераккаунтинформатион из свойства навигации учетной записи.</span><span class="sxs-lookup"><span data-stu-id="46714-115">Get the userAccountInformation resources from the account navigation property.</span></span>|
|[<span data-ttu-id="46714-116">Создание Усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="46714-116">Create userAccountInformation</span></span>](../api/profile-post-accounts.md)|[<span data-ttu-id="46714-117">усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="46714-117">userAccountInformation</span></span>](../resources/useraccountinformation.md)|<span data-ttu-id="46714-118">Создание нового объекта Усераккаунтинформатион.</span><span class="sxs-lookup"><span data-stu-id="46714-118">Create a new userAccountInformation object.</span></span>|
|[<span data-ttu-id="46714-119">Получение Усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="46714-119">Get userAccountInformation</span></span>](../api/useraccountinformation-get.md)|[<span data-ttu-id="46714-120">усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="46714-120">userAccountInformation</span></span>](../resources/useraccountinformation.md)|<span data-ttu-id="46714-121">Чтение свойств и связей объекта [усераккаунтинформатион](../resources/useraccountinformation.md) .</span><span class="sxs-lookup"><span data-stu-id="46714-121">Read the properties and relationships of a [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>|
|[<span data-ttu-id="46714-122">Обновление Усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="46714-122">Update userAccountInformation</span></span>](../api/useraccountinformation-update.md)|[<span data-ttu-id="46714-123">усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="46714-123">userAccountInformation</span></span>](../resources/useraccountinformation.md)|<span data-ttu-id="46714-124">Обновление свойств объекта [усераккаунтинформатион](../resources/useraccountinformation.md) .</span><span class="sxs-lookup"><span data-stu-id="46714-124">Update the properties of a [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>|
|[<span data-ttu-id="46714-125">Удаление Усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="46714-125">Delete userAccountInformation</span></span>](../api/useraccountinformation-delete.md)|<span data-ttu-id="46714-126">Нет</span><span class="sxs-lookup"><span data-stu-id="46714-126">None</span></span>|<span data-ttu-id="46714-127">Удаляет объект [усераккаунтинформатион](../resources/useraccountinformation.md) .</span><span class="sxs-lookup"><span data-stu-id="46714-127">Deletes a [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="46714-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="46714-128">Properties</span></span>

|<span data-ttu-id="46714-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="46714-129">Property</span></span>|<span data-ttu-id="46714-130">Тип</span><span class="sxs-lookup"><span data-stu-id="46714-130">Type</span></span>|<span data-ttu-id="46714-131">Описание</span><span class="sxs-lookup"><span data-stu-id="46714-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46714-132">ageGroup</span><span class="sxs-lookup"><span data-stu-id="46714-132">ageGroup</span></span>|<span data-ttu-id="46714-133">String</span><span class="sxs-lookup"><span data-stu-id="46714-133">String</span></span>|<span data-ttu-id="46714-134">Показывает группу возрастных пользователей.</span><span class="sxs-lookup"><span data-stu-id="46714-134">Shows the age group of user.</span></span> <span data-ttu-id="46714-135">Допустимые `null` значения `minor` , `notAdult` и `adult` они создаются каталогом и не могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="46714-135">Allowed values `null`, `minor`, `notAdult` and `adult` are generated by the directory and cannot be changed.</span></span>|
|<span data-ttu-id="46714-136">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="46714-136">allowedAudiences</span></span>|<span data-ttu-id="46714-137">String</span><span class="sxs-lookup"><span data-stu-id="46714-137">String</span></span>|<span data-ttu-id="46714-138">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="46714-138">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="46714-139">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="46714-139">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="46714-140">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="46714-140">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="46714-141">countryCode</span><span class="sxs-lookup"><span data-stu-id="46714-141">countryCode</span></span>|<span data-ttu-id="46714-142">String</span><span class="sxs-lookup"><span data-stu-id="46714-142">String</span></span>|<span data-ttu-id="46714-143">Содержит двухбуквенный код страны, связанный с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="46714-143">Contains the two-character country code associated with the users account.</span></span>  |
|<span data-ttu-id="46714-144">createdBy</span><span class="sxs-lookup"><span data-stu-id="46714-144">createdBy</span></span>|[<span data-ttu-id="46714-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="46714-145">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="46714-146">Предоставляет идентификатор пользователя и/или приложения, создавшего сущность.</span><span class="sxs-lookup"><span data-stu-id="46714-146">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="46714-147">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="46714-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="46714-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="46714-148">createdDateTime</span></span>|<span data-ttu-id="46714-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46714-149">DateTimeOffset</span></span>|<span data-ttu-id="46714-150">Предоставляет значение dateTimeOffset для объекта, когда была создана сущность.</span><span class="sxs-lookup"><span data-stu-id="46714-150">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="46714-151">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="46714-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="46714-152">id</span><span class="sxs-lookup"><span data-stu-id="46714-152">id</span></span>|<span data-ttu-id="46714-153">String</span><span class="sxs-lookup"><span data-stu-id="46714-153">String</span></span>|<span data-ttu-id="46714-154">Идентификатор, используемый для индивидуальной адресации объекта.</span><span class="sxs-lookup"><span data-stu-id="46714-154">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="46714-155">Наследуется от [объекта](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="46714-155">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="46714-156">выводов</span><span class="sxs-lookup"><span data-stu-id="46714-156">inference</span></span>|[<span data-ttu-id="46714-157">инференцедата</span><span class="sxs-lookup"><span data-stu-id="46714-157">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="46714-158">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="46714-158">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="46714-159">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="46714-159">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="46714-160">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="46714-160">lastModifiedBy</span></span>|[<span data-ttu-id="46714-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="46714-161">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="46714-162">Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект.</span><span class="sxs-lookup"><span data-stu-id="46714-162">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="46714-163">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="46714-163">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="46714-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="46714-164">lastModifiedDateTime</span></span>|<span data-ttu-id="46714-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46714-165">DateTimeOffset</span></span>|<span data-ttu-id="46714-166">Предоставляет значение dateTimeOffset для объекта, когда была создана сущность.</span><span class="sxs-lookup"><span data-stu-id="46714-166">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="46714-167">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="46714-167">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="46714-168">преферредлангуажетаг</span><span class="sxs-lookup"><span data-stu-id="46714-168">preferredLanguageTag</span></span>|[<span data-ttu-id="46714-169">localeInfo</span><span class="sxs-lookup"><span data-stu-id="46714-169">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="46714-170">Содержит язык, который пользователь связал с учетной записью как предпочитаемый.</span><span class="sxs-lookup"><span data-stu-id="46714-170">Contains the language the user has associated as preferred for the account.</span></span>   |
|<span data-ttu-id="46714-171">source</span><span class="sxs-lookup"><span data-stu-id="46714-171">source</span></span>|[<span data-ttu-id="46714-172">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="46714-172">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="46714-173">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="46714-173">Where the values originated if synced from another service.</span></span> <span data-ttu-id="46714-174">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="46714-174">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="46714-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="46714-175">userPrincipalName</span></span>|<span data-ttu-id="46714-176">String</span><span class="sxs-lookup"><span data-stu-id="46714-176">String</span></span>|<span data-ttu-id="46714-177">Имя участника-пользователя (UPN) пользователя, связанного с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="46714-177">The user principal name (UPN) of the user associated with the account.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="46714-178">Связи</span><span class="sxs-lookup"><span data-stu-id="46714-178">Relationships</span></span>
<span data-ttu-id="46714-179">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="46714-179">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="46714-180">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="46714-180">JSON representation</span></span>
<span data-ttu-id="46714-181">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46714-181">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userAccountInformation",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAccountInformation",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "ageGroup": "String",
  "countryCode": "String",
  "preferredLanguageTag": {
    "@odata.type": "microsoft.graph.localeInfo"
  },
  "userPrincipalName": "String"
}
```


