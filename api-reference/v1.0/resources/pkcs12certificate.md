---
title: тип ресурса pkcs12Certificate
description: Представляет конфигурацию для загрузки pkcs12Certificate.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 60350908901293ec9bf090c9e2bc174d70c922e5
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882443"
---
# <a name="pkcs12certificate-resource-type"></a><span data-ttu-id="19884-103">тип ресурса pkcs12Certificate</span><span class="sxs-lookup"><span data-stu-id="19884-103">pkcs12Certificate resource type</span></span>

<span data-ttu-id="19884-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19884-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="19884-105">Представляет конфигурацию, используемую для отправки сертификата при использовании проверки подлинности клиентского сертификата HTTPS для вызова конечной точки соединителя API.</span><span class="sxs-lookup"><span data-stu-id="19884-105">Represents the configuration used to upload a certificate when using HTTPS client-certificate authentication for calling an API connector endpoint.</span></span> <span data-ttu-id="19884-106">Проверка подлинности клиентского сертификата — это взаимная проверка подлинности на основе сертификата, в которой клиент предоставляет клиентский сертификат конечной точке API для проверки его подлинности.</span><span class="sxs-lookup"><span data-stu-id="19884-106">Client certificate authentication is a mutual certificate-based authentication, where the client provides a client certificate to an API endpoint to prove its identity.</span></span> <span data-ttu-id="19884-107">Настроенный сертификат соединиттеля API отправляется Azure AD в конечную точку API, которая затем проверяет сертификат.</span><span class="sxs-lookup"><span data-stu-id="19884-107">The configured certificate of an API connector is sent by Azure AD to the given API endpoint, which then validates the certificate.</span></span>

<span data-ttu-id="19884-108">Наследует [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="19884-108">Inherits from [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="19884-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="19884-109">Properties</span></span>

|<span data-ttu-id="19884-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="19884-110">Property</span></span>|<span data-ttu-id="19884-111">Тип</span><span class="sxs-lookup"><span data-stu-id="19884-111">Type</span></span>|<span data-ttu-id="19884-112">Описание</span><span class="sxs-lookup"><span data-stu-id="19884-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19884-113">pkcs12Value</span><span class="sxs-lookup"><span data-stu-id="19884-113">pkcs12Value</span></span>|<span data-ttu-id="19884-114">Строка</span><span class="sxs-lookup"><span data-stu-id="19884-114">String</span></span>| <span data-ttu-id="19884-115">Представляет отправленное содержимое pfx.</span><span class="sxs-lookup"><span data-stu-id="19884-115">Represents the pfx content that is sent.</span></span> <span data-ttu-id="19884-116">Значение должно быть кодированной версией базового-64 фактического контента сертификата.</span><span class="sxs-lookup"><span data-stu-id="19884-116">The value should be a base-64 encoded version of the actual certificate content.</span></span> <span data-ttu-id="19884-117">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="19884-117">Required.</span></span>|
|<span data-ttu-id="19884-118">password</span><span class="sxs-lookup"><span data-stu-id="19884-118">password</span></span>|<span data-ttu-id="19884-119">Строка</span><span class="sxs-lookup"><span data-stu-id="19884-119">String</span></span>| <span data-ttu-id="19884-120">Пароль для файла pfx.</span><span class="sxs-lookup"><span data-stu-id="19884-120">The password for the pfx file.</span></span> <span data-ttu-id="19884-121">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="19884-121">Required.</span></span> <span data-ttu-id="19884-122">Если пароль не используется, необходимо предоставить значение `""` .</span><span class="sxs-lookup"><span data-stu-id="19884-122">If no password is used, you must still provide a value of `""`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="19884-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19884-123">JSON representation</span></span>

<span data-ttu-id="19884-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19884-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.pkcs12Certificate"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.pkcs12Certificate",
  "pkcs12Value": "String",
  "password": "String"
}
```
