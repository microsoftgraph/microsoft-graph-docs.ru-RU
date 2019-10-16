---
title: Тип ресурса Цертификатебаседаусконфигуратион
description: Представляет коллекцию центров сертификации.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d0b5b57a7594dfaf4fde88615c6a21314618c0eb
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539290"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a><span data-ttu-id="c70b9-103">Тип ресурса Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="c70b9-103">certificateBasedAuthConfiguration resource type</span></span>

<span data-ttu-id="c70b9-104">Проверка подлинности на основе сертификатов обеспечивает проверку подлинности Azure Active Directory с помощью сертификата клиента на устройстве Windows, Android или iOS при подключении учетной записи Exchange Online к:</span><span class="sxs-lookup"><span data-stu-id="c70b9-104">Certificate-based authentication enables you to be authenticated by Azure Active Directory with a client certificate on a Windows, Android, or iOS device when connecting your Exchange Online account to:</span></span>

- <span data-ttu-id="c70b9-105">Мобильные приложения Майкрософт, такие как Outlook и Word</span><span class="sxs-lookup"><span data-stu-id="c70b9-105">Microsoft mobile applications such as Outlook and Word</span></span>
- <span data-ttu-id="c70b9-106">Клиенты Exchange ActiveSync (EAS)</span><span class="sxs-lookup"><span data-stu-id="c70b9-106">Exchange ActiveSync (EAS) clients</span></span>

<span data-ttu-id="c70b9-107">Настройка этой функции исключает необходимость ввода имени пользователя и пароля в определенные приложения электронной почты и приложения Microsoft Office на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="c70b9-107">Configuring this feature eliminates the need to enter a username and password combination into certain mail and Microsoft Office applications on your mobile device.</span></span>

<span data-ttu-id="c70b9-108">Настройка проверки подлинности на основе сертификатов обеспечивается через коллекцию центров сертификации.</span><span class="sxs-lookup"><span data-stu-id="c70b9-108">Certificate-based authentication configuration is provided through a collection of certificate authorities.</span></span> <span data-ttu-id="c70b9-109">Центры сертификации используются для установки доверенной цепочки сертификатов, что позволяет клиентам выполнять проверку подлинности с помощью Azure Active Directory с помощью сертификата клиента.</span><span class="sxs-lookup"><span data-stu-id="c70b9-109">The certificate authorities are used to establish a trusted certificate chain which enables clients to be authenticated by Azure Active Directory with a client certificate.</span></span>

<span data-ttu-id="c70b9-110">Узнайте больше о [проверке подлинности на основе сертификатов в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).</span><span class="sxs-lookup"><span data-stu-id="c70b9-110">Learn more about [certificate-based authentication in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).</span></span>

## <a name="methods"></a><span data-ttu-id="c70b9-111">Методы</span><span class="sxs-lookup"><span data-stu-id="c70b9-111">Methods</span></span>

| <span data-ttu-id="c70b9-112">Метод</span><span class="sxs-lookup"><span data-stu-id="c70b9-112">Method</span></span>       | <span data-ttu-id="c70b9-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c70b9-113">Return Type</span></span> | <span data-ttu-id="c70b9-114">Описание</span><span class="sxs-lookup"><span data-stu-id="c70b9-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c70b9-115">Список Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="c70b9-115">List certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-list.md) | [<span data-ttu-id="c70b9-116">цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="c70b9-116">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="c70b9-117">Перечисление свойств коллекции **цертификатебаседаусконфигуратион** .</span><span class="sxs-lookup"><span data-stu-id="c70b9-117">List the properties of the **certificateBasedAuthConfiguration** collection.</span></span> |
| [<span data-ttu-id="c70b9-118">Создание Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="c70b9-118">Create certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [<span data-ttu-id="c70b9-119">цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="c70b9-119">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="c70b9-120">Создание нового объекта **цертификатебаседаусконфигуратион** .</span><span class="sxs-lookup"><span data-stu-id="c70b9-120">Create a new **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="c70b9-121">Получение Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="c70b9-121">Get certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-get.md) | [<span data-ttu-id="c70b9-122">цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="c70b9-122">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="c70b9-123">Чтение свойств объекта **цертификатебаседаусконфигуратион** .</span><span class="sxs-lookup"><span data-stu-id="c70b9-123">Read the properties of a **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="c70b9-124">Удаление Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="c70b9-124">Delete certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-delete.md) | <span data-ttu-id="c70b9-125">Нет</span><span class="sxs-lookup"><span data-stu-id="c70b9-125">None</span></span> | <span data-ttu-id="c70b9-126">Удаление объекта **цертификатебаседаусконфигуратион** .</span><span class="sxs-lookup"><span data-stu-id="c70b9-126">Delete a **certificateBasedAuthConfiguration** object.</span></span> |

>[!NOTE]
><span data-ttu-id="c70b9-127">Обновление **церфикатебаседаусконфигуратион** не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c70b9-127">Updating **cerficateBasedAuthConfiguration** is not supported.</span></span> <span data-ttu-id="c70b9-128">Чтобы изменить **церфикатебаседаусконфигуратион**, сначала удалите его, а затем создайте новый **церфикатебаседаусконфигуратион**.</span><span class="sxs-lookup"><span data-stu-id="c70b9-128">To change a **cerficateBasedAuthConfiguration**, first delete and then create a new **cerficateBasedAuthConfiguration**.</span></span>

## <a name="properties"></a><span data-ttu-id="c70b9-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="c70b9-129">Properties</span></span>

| <span data-ttu-id="c70b9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c70b9-130">Property</span></span>     | <span data-ttu-id="c70b9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c70b9-131">Type</span></span>        | <span data-ttu-id="c70b9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c70b9-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c70b9-133">цертификатеаусоритиес</span><span class="sxs-lookup"><span data-stu-id="c70b9-133">certificateAuthorities</span></span>|<span data-ttu-id="c70b9-134">Коллекция [цертификатеаусорити](certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="c70b9-134">[certificateAuthority](certificateauthority.md) collection</span></span>|<span data-ttu-id="c70b9-135">Коллекция центров сертификации, которая создает доверенную цепочку сертификатов.</span><span class="sxs-lookup"><span data-stu-id="c70b9-135">Collection of certificate authorities which creates a trusted certificate chain.</span></span>|
|<span data-ttu-id="c70b9-136">id</span><span class="sxs-lookup"><span data-stu-id="c70b9-136">id</span></span>|<span data-ttu-id="c70b9-137">String</span><span class="sxs-lookup"><span data-stu-id="c70b9-137">String</span></span>|<span data-ttu-id="c70b9-138">Уникальный идентификатор конфигурации проверки подлинности на основе сертификатов.</span><span class="sxs-lookup"><span data-stu-id="c70b9-138">The unique identifier of the certificate based auth configuration.</span></span> <span data-ttu-id="c70b9-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c70b9-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c70b9-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="c70b9-140">Relationships</span></span>

<span data-ttu-id="c70b9-141">Нет</span><span class="sxs-lookup"><span data-stu-id="c70b9-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c70b9-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c70b9-142">JSON representation</span></span>

<span data-ttu-id="c70b9-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c70b9-143">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "certificateAuthorities": {"@odata.type": "collection(microsoft.graph.certificateAuthority)"},
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "certificateBasedAuthConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
