---
title: тип ресурса pkcs12Certificate
description: Представляет конфигурацию для загрузки pkcs12Certificate в вызове API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f312a7be0bd29d57c1a6b7dc5c7e5d72e6d41206
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509404"
---
# <a name="pkcs12certificate-resource-type"></a><span data-ttu-id="ad4b4-103">тип ресурса pkcs12Certificate</span><span class="sxs-lookup"><span data-stu-id="ad4b4-103">pkcs12Certificate resource type</span></span>

<span data-ttu-id="ad4b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad4b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad4b4-105">Представляет конфигурацию, используемую **для** отправки сертификата при использовании проверки подлинности клиентского сертификата HTTPS для вызова конечной точки соединителя API.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-105">Represents the configuration used to **upload** a certificate when using HTTPS client-certificate authentication for calling an API connector endpoint.</span></span> <span data-ttu-id="ad4b4-106">Проверка подлинности клиентского сертификата — это взаимная проверка подлинности на основе сертификата, в которой клиент предоставляет клиентский сертификат конечной точке API для проверки его подлинности.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-106">Client certificate authentication is a mutual certificate-based authentication, where the client provides a client certificate to an API endpoint to prove its identity.</span></span> <span data-ttu-id="ad4b4-107">Настроенный сертификат соединиттеля API отправляется Azure AD в конечную точку API, которая затем проверяет сертификат.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-107">The configured certificate of an API connector is sent by Azure AD to the given API endpoint, which then validates the certificate.</span></span>

<span data-ttu-id="ad4b4-108">Наследует [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="ad4b4-108">Inherits from [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ad4b4-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad4b4-109">Properties</span></span>

|<span data-ttu-id="ad4b4-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad4b4-110">Property</span></span>|<span data-ttu-id="ad4b4-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ad4b4-111">Type</span></span>|<span data-ttu-id="ad4b4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ad4b4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad4b4-113">pkcs12Value</span><span class="sxs-lookup"><span data-stu-id="ad4b4-113">pkcs12Value</span></span>|<span data-ttu-id="ad4b4-114">String</span><span class="sxs-lookup"><span data-stu-id="ad4b4-114">String</span></span>| <span data-ttu-id="ad4b4-115">Это поле для отправки контента pfx.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-115">This is the field for sending pfx content.</span></span> <span data-ttu-id="ad4b4-116">Значение должно быть кодированной версией базового-64 фактического контента сертификата.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-116">The value should be a base-64 encoded version of the actual certificate content.</span></span> <span data-ttu-id="ad4b4-117">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-117">Required.</span></span>|
|<span data-ttu-id="ad4b4-118">password</span><span class="sxs-lookup"><span data-stu-id="ad4b4-118">password</span></span>|<span data-ttu-id="ad4b4-119">Строка</span><span class="sxs-lookup"><span data-stu-id="ad4b4-119">String</span></span>| <span data-ttu-id="ad4b4-120">Это пароль для файла pfx.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-120">This is the password for the pfx file.</span></span> <span data-ttu-id="ad4b4-121">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-121">Required.</span></span> <span data-ttu-id="ad4b4-122">Если пароль не используется, необходимо по-прежнему предоставлять значение `""` .</span><span class="sxs-lookup"><span data-stu-id="ad4b4-122">If no password is used, must still provide a value of `""`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad4b4-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad4b4-123">JSON representation</span></span>

<span data-ttu-id="ad4b4-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad4b4-124">The following is a JSON representation of the resource.</span></span>
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
