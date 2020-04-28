---
title: Тип ресурса Токениссуанцеполици
description: Представляет политику, определяющую характеристики маркеров SAML, выданных Azure AD.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ecd776364fbdc3dcd0b4dbf59ff60c8e6624262b
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917371"
---
# <a name="tokenissuancepolicy-resource-type"></a><span data-ttu-id="8a0c7-103">Тип ресурса Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="8a0c7-103">tokenIssuancePolicy resource type</span></span>

<span data-ttu-id="8a0c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a0c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a0c7-105">Представляет политику, определяющую характеристики маркеров SAML, выданных Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-105">Represents the policy to specify the characteristics of SAML tokens issued by Azure AD.</span></span> <span data-ttu-id="8a0c7-106">Политики выдачи маркеров можно использовать для следующих действий:</span><span class="sxs-lookup"><span data-stu-id="8a0c7-106">You can use token-issuance policies to:</span></span>

- <span data-ttu-id="8a0c7-107">Настройка параметров подписывания</span><span class="sxs-lookup"><span data-stu-id="8a0c7-107">Set signing options</span></span>
- <span data-ttu-id="8a0c7-108">Настройка алгоритма подписи</span><span class="sxs-lookup"><span data-stu-id="8a0c7-108">Set signing algorithm</span></span>
- <span data-ttu-id="8a0c7-109">Установка версии токена SAML</span><span class="sxs-lookup"><span data-stu-id="8a0c7-109">Set SAML token version</span></span>

<span data-ttu-id="8a0c7-110">Наследуется от [стсполици](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8a0c7-110">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8a0c7-111">Методы</span><span class="sxs-lookup"><span data-stu-id="8a0c7-111">Methods</span></span>

| <span data-ttu-id="8a0c7-112">Метод</span><span class="sxs-lookup"><span data-stu-id="8a0c7-112">Method</span></span>       | <span data-ttu-id="8a0c7-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8a0c7-113">Return Type</span></span> | <span data-ttu-id="8a0c7-114">Описание</span><span class="sxs-lookup"><span data-stu-id="8a0c7-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8a0c7-115">Создание Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="8a0c7-115">Create tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-post-tokenissuancepolicy.md) | [<span data-ttu-id="8a0c7-116">токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="8a0c7-116">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="8a0c7-117">Создание объекта Токениссуанцеполици.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-117">Create a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="8a0c7-118">Получение Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="8a0c7-118">Get tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-get.md) | [<span data-ttu-id="8a0c7-119">токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="8a0c7-119">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="8a0c7-120">Чтение свойств и связей объекта Токениссуанцеполици.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-120">Read properties and relationships of a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="8a0c7-121">Список Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="8a0c7-121">List tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-list.md) | [<span data-ttu-id="8a0c7-122">токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="8a0c7-122">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="8a0c7-123">Чтение свойств и связей объектов Токениссуанцеполици.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-123">Read properties and relationships of tokenIssuancePolicy objects.</span></span> |
| [<span data-ttu-id="8a0c7-124">Обновление Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="8a0c7-124">Update tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-update.md) | <span data-ttu-id="8a0c7-125">Нет</span><span class="sxs-lookup"><span data-stu-id="8a0c7-125">None</span></span> | <span data-ttu-id="8a0c7-126">Обновление объекта Токениссуанцеполици.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-126">Update a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="8a0c7-127">Удаление Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="8a0c7-127">Delete tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-delete.md) | <span data-ttu-id="8a0c7-128">Нет</span><span class="sxs-lookup"><span data-stu-id="8a0c7-128">None</span></span> | <span data-ttu-id="8a0c7-129">Удаление объекта Токениссуанцеполици.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-129">Delete a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="8a0c7-130">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="8a0c7-130">List appliesTo</span></span>](../api/tokenissuancepolicy-list-appliesto.md) | <span data-ttu-id="8a0c7-131">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="8a0c7-131">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="8a0c7-132">Получение списка Директорйобжектс, к которым применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-132">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="8a0c7-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a0c7-133">Properties</span></span>

| <span data-ttu-id="8a0c7-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a0c7-134">Property</span></span>     | <span data-ttu-id="8a0c7-135">Тип</span><span class="sxs-lookup"><span data-stu-id="8a0c7-135">Type</span></span>        | <span data-ttu-id="8a0c7-136">Описание</span><span class="sxs-lookup"><span data-stu-id="8a0c7-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8a0c7-137">id</span><span class="sxs-lookup"><span data-stu-id="8a0c7-137">id</span></span>|<span data-ttu-id="8a0c7-138">String</span><span class="sxs-lookup"><span data-stu-id="8a0c7-138">String</span></span>| <span data-ttu-id="8a0c7-139">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-139">Unique identifier for this policy.</span></span> <span data-ttu-id="8a0c7-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-140">Read-only.</span></span>|
|<span data-ttu-id="8a0c7-141">RDLC</span><span class="sxs-lookup"><span data-stu-id="8a0c7-141">definition</span></span>|<span data-ttu-id="8a0c7-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="8a0c7-142">String collection</span></span>| <span data-ttu-id="8a0c7-143">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-143">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="8a0c7-144">Ниже приведены дополнительные сведения о схеме JSON для этого свойства.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-144">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="8a0c7-145">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-145">Required.</span></span>|
|<span data-ttu-id="8a0c7-146">description</span><span class="sxs-lookup"><span data-stu-id="8a0c7-146">description</span></span>|<span data-ttu-id="8a0c7-147">String</span><span class="sxs-lookup"><span data-stu-id="8a0c7-147">String</span></span>| <span data-ttu-id="8a0c7-148">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-148">Description for this policy.</span></span>|
|<span data-ttu-id="8a0c7-149">displayName</span><span class="sxs-lookup"><span data-stu-id="8a0c7-149">displayName</span></span>|<span data-ttu-id="8a0c7-150">Строка</span><span class="sxs-lookup"><span data-stu-id="8a0c7-150">String</span></span>| <span data-ttu-id="8a0c7-151">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-151">Display name for this policy.</span></span> <span data-ttu-id="8a0c7-152">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-152">Required.</span></span>|
|<span data-ttu-id="8a0c7-153">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="8a0c7-153">isOrganizationDefault</span></span>|<span data-ttu-id="8a0c7-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a0c7-154">Boolean</span></span>|<span data-ttu-id="8a0c7-155">Игнорировать это свойство.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-155">Ignore this property.</span></span> <span data-ttu-id="8a0c7-156">Политика выдачи маркеров может применяться только к субъектам служб и не может быть настроена глобально для Организации.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-156">The token-issuance policy can only be applied to service principals and can't be set globally for the organization.</span></span>|


### <a name="properties-of-a-token-issuance-policy-definition"></a><span data-ttu-id="8a0c7-157">Свойства определения политики выдачи маркеров</span><span class="sxs-lookup"><span data-stu-id="8a0c7-157">Properties of a token issuance policy definition</span></span>
<span data-ttu-id="8a0c7-158">Свойства формируют объект JSON, представляющий политику выдачи маркеров.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-158">The properties form the JSON object that represents a token issuance policy.</span></span> <span data-ttu-id="8a0c7-159">Этот объект JSON необходимо **преобразовать в строку с escape-символами** , которые будут вставлены в свойство **definition** .</span><span class="sxs-lookup"><span data-stu-id="8a0c7-159">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="8a0c7-160">Ниже приведен пример в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-160">The following is an example in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{ \"TokenIssuancePolicy\":{\"TokenResponseSigningPolicy\":\"TokenOnly\",\"SamlTokenVersion\":\"1.1\",\"SigningAlgorithm\":\"http://www.w3.org/2001/04/xmldsig-more#rsa-sha256\",\"Version\":1}}"
  ]
```


| <span data-ttu-id="8a0c7-161">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a0c7-161">Property</span></span>     | <span data-ttu-id="8a0c7-162">Тип</span><span class="sxs-lookup"><span data-stu-id="8a0c7-162">Type</span></span>   |<span data-ttu-id="8a0c7-163">Описание</span><span class="sxs-lookup"><span data-stu-id="8a0c7-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a0c7-164">токенреспонсесигнингполици</span><span class="sxs-lookup"><span data-stu-id="8a0c7-164">TokenResponseSigningPolicy</span></span>|<span data-ttu-id="8a0c7-165">String</span><span class="sxs-lookup"><span data-stu-id="8a0c7-165">String</span></span>|<span data-ttu-id="8a0c7-166">Представляет параметры подписи сертификатов, доступные в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-166">Represents the certificate signing options available in Azure AD.</span></span> <span data-ttu-id="8a0c7-167">Поддерживаются следующие значения `ResponseOnly`: `TokenOnly`, `ResponseAndToken`,.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-167">Supported values are: `ResponseOnly`, `TokenOnly`, `ResponseAndToken`.</span></span>  |
|<span data-ttu-id="8a0c7-168">самлтокенверсион</span><span class="sxs-lookup"><span data-stu-id="8a0c7-168">SamlTokenVersion</span></span>|<span data-ttu-id="8a0c7-169">String</span><span class="sxs-lookup"><span data-stu-id="8a0c7-169">String</span></span>|<span data-ttu-id="8a0c7-170">Версия маркера SAML.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-170">Version of the SAML token.</span></span> <span data-ttu-id="8a0c7-171">Поддерживаются следующие значения `1.1`: `2.0`,.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-171">Supported values are: `1.1`, `2.0`.</span></span> |
|<span data-ttu-id="8a0c7-172">сигнингалгорисм</span><span class="sxs-lookup"><span data-stu-id="8a0c7-172">SigningAlgorithm</span></span>|<span data-ttu-id="8a0c7-173">String</span><span class="sxs-lookup"><span data-stu-id="8a0c7-173">String</span></span>|<span data-ttu-id="8a0c7-174">Использование алгоритма подписи для подписи маркера SAML в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-174">Signing algorithm use by Azure AD to sign the SAML token.</span></span> <span data-ttu-id="8a0c7-175">Поддерживаются следующие значения `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256`: `http://www.w3.org/2000/09/xmldsig#rsa-sha1`,.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-175">Supported values are: `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256`, `http://www.w3.org/2000/09/xmldsig#rsa-sha1`.</span></span>|
|<span data-ttu-id="8a0c7-176">Версия</span><span class="sxs-lookup"><span data-stu-id="8a0c7-176">Version</span></span>|<span data-ttu-id="8a0c7-177">Целое число</span><span class="sxs-lookup"><span data-stu-id="8a0c7-177">Integer</span></span>|<span data-ttu-id="8a0c7-178">Установите значение 1.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-178">Set value of 1.</span></span> <span data-ttu-id="8a0c7-179">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-179">Required.</span></span>|


## <a name="relationships"></a><span data-ttu-id="8a0c7-180">Связи</span><span class="sxs-lookup"><span data-stu-id="8a0c7-180">Relationships</span></span>

| <span data-ttu-id="8a0c7-181">Связь</span><span class="sxs-lookup"><span data-stu-id="8a0c7-181">Relationship</span></span> | <span data-ttu-id="8a0c7-182">Тип</span><span class="sxs-lookup"><span data-stu-id="8a0c7-182">Type</span></span>        | <span data-ttu-id="8a0c7-183">Описание</span><span class="sxs-lookup"><span data-stu-id="8a0c7-183">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8a0c7-184">Тег</span><span class="sxs-lookup"><span data-stu-id="8a0c7-184">appliesTo</span></span>|<span data-ttu-id="8a0c7-185">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="8a0c7-185">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="8a0c7-186">Коллекция [directoryObject](directoryObject.md) , к которой применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-186">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="8a0c7-187">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-187">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8a0c7-188">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a0c7-188">JSON representation</span></span>

<span data-ttu-id="8a0c7-189">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a0c7-189">The following is a JSON representation of the resource.</span></span>

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
