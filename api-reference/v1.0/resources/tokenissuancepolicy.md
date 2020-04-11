---
title: Тип ресурса Токениссуанцеполици
description: Представляет политику, определяющую характеристики маркеров SAML, выданных Azure AD.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 030b05a7609b9588f0860471272c62007eaa1692
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229579"
---
# <a name="tokenissuancepolicy-resource-type"></a><span data-ttu-id="eb6ba-103">Тип ресурса Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="eb6ba-103">tokenIssuancePolicy resource type</span></span>

<span data-ttu-id="eb6ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb6ba-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="eb6ba-105">Представляет политику, определяющую характеристики маркеров SAML, выданных Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-105">Represents the policy to specify the characteristics of SAML tokens issued by Azure AD.</span></span> <span data-ttu-id="eb6ba-106">Политики выдачи маркеров можно использовать для следующих действий:</span><span class="sxs-lookup"><span data-stu-id="eb6ba-106">You can use token-issuance policies to:</span></span>

- <span data-ttu-id="eb6ba-107">Настройка параметров подписывания</span><span class="sxs-lookup"><span data-stu-id="eb6ba-107">Set signing options</span></span>
- <span data-ttu-id="eb6ba-108">Настройка алгоритма подписи</span><span class="sxs-lookup"><span data-stu-id="eb6ba-108">Set signing algorithm</span></span>
- <span data-ttu-id="eb6ba-109">Установка версии токена SAML</span><span class="sxs-lookup"><span data-stu-id="eb6ba-109">Set SAML token version</span></span>

<span data-ttu-id="eb6ba-110">Наследуется от [стсполици](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="eb6ba-110">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="eb6ba-111">Методы</span><span class="sxs-lookup"><span data-stu-id="eb6ba-111">Methods</span></span>

| <span data-ttu-id="eb6ba-112">Метод</span><span class="sxs-lookup"><span data-stu-id="eb6ba-112">Method</span></span>       | <span data-ttu-id="eb6ba-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eb6ba-113">Return Type</span></span> | <span data-ttu-id="eb6ba-114">Описание</span><span class="sxs-lookup"><span data-stu-id="eb6ba-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="eb6ba-115">Список Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="eb6ba-115">List tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-list.md) | [<span data-ttu-id="eb6ba-116">токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="eb6ba-116">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="eb6ba-117">Чтение свойств и связей объектов Токениссуанцеполици.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-117">Read properties and relationships of tokenIssuancePolicy objects.</span></span> |
| [<span data-ttu-id="eb6ba-118">Создание Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="eb6ba-118">Create tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-post-tokenissuancepolicy.md) | [<span data-ttu-id="eb6ba-119">токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="eb6ba-119">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="eb6ba-120">Создание объекта Токениссуанцеполици.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-120">Create a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="eb6ba-121">Получение Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="eb6ba-121">Get tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-get.md) | [<span data-ttu-id="eb6ba-122">токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="eb6ba-122">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="eb6ba-123">Чтение свойств и связей объекта Токениссуанцеполици.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-123">Read properties and relationships of a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="eb6ba-124">Обновление Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="eb6ba-124">Update tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-update.md) | <span data-ttu-id="eb6ba-125">Нет</span><span class="sxs-lookup"><span data-stu-id="eb6ba-125">None</span></span> | <span data-ttu-id="eb6ba-126">Обновление объекта Токениссуанцеполици.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-126">Update a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="eb6ba-127">Удаление Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="eb6ba-127">Delete tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-delete.md) | <span data-ttu-id="eb6ba-128">Нет</span><span class="sxs-lookup"><span data-stu-id="eb6ba-128">None</span></span> | <span data-ttu-id="eb6ba-129">Удаление объекта Токениссуанцеполици.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-129">Delete a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="eb6ba-130">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="eb6ba-130">List appliesTo</span></span>](../api/tokenissuancepolicy-list-appliesto.md) | <span data-ttu-id="eb6ba-131">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="eb6ba-131">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="eb6ba-132">Получение списка Директорйобжектс, к которым применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-132">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="eb6ba-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb6ba-133">Properties</span></span>

| <span data-ttu-id="eb6ba-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb6ba-134">Property</span></span>     | <span data-ttu-id="eb6ba-135">Тип</span><span class="sxs-lookup"><span data-stu-id="eb6ba-135">Type</span></span>        | <span data-ttu-id="eb6ba-136">Описание</span><span class="sxs-lookup"><span data-stu-id="eb6ba-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eb6ba-137">id</span><span class="sxs-lookup"><span data-stu-id="eb6ba-137">id</span></span>|<span data-ttu-id="eb6ba-138">String</span><span class="sxs-lookup"><span data-stu-id="eb6ba-138">String</span></span>| <span data-ttu-id="eb6ba-139">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-139">Unique identifier for this policy.</span></span> <span data-ttu-id="eb6ba-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-140">Read-only.</span></span>|
|<span data-ttu-id="eb6ba-141">RDLC</span><span class="sxs-lookup"><span data-stu-id="eb6ba-141">definition</span></span>|<span data-ttu-id="eb6ba-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="eb6ba-142">String collection</span></span>| <span data-ttu-id="eb6ba-143">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-143">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="eb6ba-144">Ниже приведены дополнительные сведения о схеме JSON для этого свойства.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-144">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="eb6ba-145">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-145">Required.</span></span>|
|<span data-ttu-id="eb6ba-146">description</span><span class="sxs-lookup"><span data-stu-id="eb6ba-146">description</span></span>|<span data-ttu-id="eb6ba-147">String</span><span class="sxs-lookup"><span data-stu-id="eb6ba-147">String</span></span>| <span data-ttu-id="eb6ba-148">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-148">Description for this policy.</span></span>|
|<span data-ttu-id="eb6ba-149">displayName</span><span class="sxs-lookup"><span data-stu-id="eb6ba-149">displayName</span></span>|<span data-ttu-id="eb6ba-150">Строка</span><span class="sxs-lookup"><span data-stu-id="eb6ba-150">String</span></span>| <span data-ttu-id="eb6ba-151">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-151">Display name for this policy.</span></span> <span data-ttu-id="eb6ba-152">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-152">Required.</span></span>|
|<span data-ttu-id="eb6ba-153">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="eb6ba-153">isOrganizationDefault</span></span>|<span data-ttu-id="eb6ba-154">Логический</span><span class="sxs-lookup"><span data-stu-id="eb6ba-154">Boolean</span></span>|<span data-ttu-id="eb6ba-155">Игнорировать это свойство.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-155">Ignore this property.</span></span> <span data-ttu-id="eb6ba-156">Политика выдачи маркеров может применяться только к субъектам служб и не может быть настроена глобально для Организации.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-156">The token-issuance policy can only be applied to service principals and can't be set globally for the organization.</span></span>|


### <a name="properties-of-a-token-issuance-policy-definition"></a><span data-ttu-id="eb6ba-157">Свойства определения политики выдачи маркеров</span><span class="sxs-lookup"><span data-stu-id="eb6ba-157">Properties of a token issuance policy definition</span></span>
<span data-ttu-id="eb6ba-158">Свойства формируют объект JSON, представляющий политику выдачи маркеров.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-158">The properties form the JSON object that represents a token issuance policy.</span></span> <span data-ttu-id="eb6ba-159">Этот объект JSON необходимо **преобразовать в строку с escape-символами** , которые будут вставлены в свойство **definition** .</span><span class="sxs-lookup"><span data-stu-id="eb6ba-159">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="eb6ba-160">Ниже приведен пример в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-160">The following is an example in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{ \"TokenIssuancePolicy\":{\"TokenResponseSigningPolicy\":\"TokenOnly\",\"SamlTokenVersion\":\"1.1\",\"SigningAlgorithm\":\"http://www.w3.org/2001/04/xmldsig-more#rsa-sha256\",\"Version\":1}}"
  ]
```


| <span data-ttu-id="eb6ba-161">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb6ba-161">Property</span></span>     | <span data-ttu-id="eb6ba-162">Тип</span><span class="sxs-lookup"><span data-stu-id="eb6ba-162">Type</span></span>   |<span data-ttu-id="eb6ba-163">Описание</span><span class="sxs-lookup"><span data-stu-id="eb6ba-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb6ba-164">токенреспонсесигнингполици</span><span class="sxs-lookup"><span data-stu-id="eb6ba-164">TokenResponseSigningPolicy</span></span>|<span data-ttu-id="eb6ba-165">String</span><span class="sxs-lookup"><span data-stu-id="eb6ba-165">String</span></span>|<span data-ttu-id="eb6ba-166">Представляет параметры подписи сертификатов, доступные в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-166">Represents the certificate signing options available in Azure AD.</span></span> <span data-ttu-id="eb6ba-167">Поддерживаются следующие значения `ResponseOnly`: `TokenOnly`, `ResponseAndToken`,.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-167">Supported values are: `ResponseOnly`, `TokenOnly`, `ResponseAndToken`.</span></span>  |
|<span data-ttu-id="eb6ba-168">самлтокенверсион</span><span class="sxs-lookup"><span data-stu-id="eb6ba-168">SamlTokenVersion</span></span>|<span data-ttu-id="eb6ba-169">String</span><span class="sxs-lookup"><span data-stu-id="eb6ba-169">String</span></span>|<span data-ttu-id="eb6ba-170">Версия маркера SAML.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-170">Version of the SAML token.</span></span> <span data-ttu-id="eb6ba-171">Поддерживаются следующие значения `1.1`: `2.0`,.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-171">Supported values are: `1.1`, `2.0`.</span></span> |
|<span data-ttu-id="eb6ba-172">сигнингалгорисм</span><span class="sxs-lookup"><span data-stu-id="eb6ba-172">SigningAlgorithm</span></span>|<span data-ttu-id="eb6ba-173">String</span><span class="sxs-lookup"><span data-stu-id="eb6ba-173">String</span></span>|<span data-ttu-id="eb6ba-174">Использование алгоритма подписи для подписи маркера SAML в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-174">Signing algorithm use by Azure AD to sign the SAML token.</span></span> <span data-ttu-id="eb6ba-175">Поддерживаются следующие значения `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256`: `http://www.w3.org/2000/09/xmldsig#rsa-sha1`,.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-175">Supported values are: `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256`, `http://www.w3.org/2000/09/xmldsig#rsa-sha1`.</span></span>|
|<span data-ttu-id="eb6ba-176">Версия</span><span class="sxs-lookup"><span data-stu-id="eb6ba-176">Version</span></span>|<span data-ttu-id="eb6ba-177">Целое число</span><span class="sxs-lookup"><span data-stu-id="eb6ba-177">Integer</span></span>|<span data-ttu-id="eb6ba-178">Установите значение 1.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-178">Set value of 1.</span></span> <span data-ttu-id="eb6ba-179">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-179">Required.</span></span>|


## <a name="relationships"></a><span data-ttu-id="eb6ba-180">Связи</span><span class="sxs-lookup"><span data-stu-id="eb6ba-180">Relationships</span></span>

| <span data-ttu-id="eb6ba-181">Связь</span><span class="sxs-lookup"><span data-stu-id="eb6ba-181">Relationship</span></span> | <span data-ttu-id="eb6ba-182">Тип</span><span class="sxs-lookup"><span data-stu-id="eb6ba-182">Type</span></span>        | <span data-ttu-id="eb6ba-183">Описание</span><span class="sxs-lookup"><span data-stu-id="eb6ba-183">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eb6ba-184">Тег</span><span class="sxs-lookup"><span data-stu-id="eb6ba-184">appliesTo</span></span>|<span data-ttu-id="eb6ba-185">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="eb6ba-185">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="eb6ba-186">Коллекция [directoryObject](directoryObject.md) , к которой применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-186">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="eb6ba-187">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-187">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eb6ba-188">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb6ba-188">JSON representation</span></span>

<span data-ttu-id="eb6ba-189">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb6ba-189">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": true,
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tokenIssuancePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
