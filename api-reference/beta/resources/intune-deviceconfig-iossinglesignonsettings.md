---
title: Тип ресурса iosSingleSignOnSettings
description: операций ввода-вывода параметров проверки подлинности Kerberos для единого входа
ms.openlocfilehash: a63848dc27afd037a6834a67c0736f86c06ac1fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081292"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="39aeb-103">Тип ресурса iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="39aeb-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="39aeb-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="39aeb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39aeb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39aeb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39aeb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="39aeb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39aeb-107">операций ввода-вывода параметров проверки подлинности Kerberos для единого входа</span><span class="sxs-lookup"><span data-stu-id="39aeb-107">iOS Kerberos authentication settings for single sign-on</span></span>
## <a name="properties"></a><span data-ttu-id="39aeb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="39aeb-108">Properties</span></span>
|<span data-ttu-id="39aeb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="39aeb-109">Property</span></span>|<span data-ttu-id="39aeb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="39aeb-110">Type</span></span>|<span data-ttu-id="39aeb-111">Description</span><span class="sxs-lookup"><span data-stu-id="39aeb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39aeb-112">allowedAppsList</span><span class="sxs-lookup"><span data-stu-id="39aeb-112">allowedAppsList</span></span>|<span data-ttu-id="39aeb-113">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="39aeb-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="39aeb-114">Список идентификаторов приложения, которые могут использовать это имя входа.</span><span class="sxs-lookup"><span data-stu-id="39aeb-114">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="39aeb-115">Если это поле указан, имя входа применяется ко всем приложениям на устройстве.</span><span class="sxs-lookup"><span data-stu-id="39aeb-115">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="39aeb-116">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="39aeb-116">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="39aeb-117">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="39aeb-117">allowedUrls</span></span>|<span data-ttu-id="39aeb-118">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="39aeb-118">String collection</span></span>|<span data-ttu-id="39aeb-119">Список URL-адресов HTTP для соответствия для использования этим именем входа.</span><span class="sxs-lookup"><span data-stu-id="39aeb-119">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="39aeb-120">С помощью операций ввода-вывода 9.0 или более поздней версии могут быть использованы подстановочные знаки.</span><span class="sxs-lookup"><span data-stu-id="39aeb-120">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="39aeb-121">displayName</span><span class="sxs-lookup"><span data-stu-id="39aeb-121">displayName</span></span>|<span data-ttu-id="39aeb-122">String</span><span class="sxs-lookup"><span data-stu-id="39aeb-122">String</span></span>|<span data-ttu-id="39aeb-123">Отображаемое имя параметры входа в систему на получающей устройства.</span><span class="sxs-lookup"><span data-stu-id="39aeb-123">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="39aeb-124">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="39aeb-124">kerberosPrincipalName</span></span>|<span data-ttu-id="39aeb-125">String</span><span class="sxs-lookup"><span data-stu-id="39aeb-125">String</span></span>|<span data-ttu-id="39aeb-126">Имя участника Kerberos.</span><span class="sxs-lookup"><span data-stu-id="39aeb-126">A Kerberos principal name.</span></span> <span data-ttu-id="39aeb-127">Если этот параметр не указан, пользователю предлагается ввести один во время установки профиля.</span><span class="sxs-lookup"><span data-stu-id="39aeb-127">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="39aeb-128">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="39aeb-128">kerberosRealm</span></span>|<span data-ttu-id="39aeb-129">String</span><span class="sxs-lookup"><span data-stu-id="39aeb-129">String</span></span>|<span data-ttu-id="39aeb-130">Имя сферы Kerberos.</span><span class="sxs-lookup"><span data-stu-id="39aeb-130">A Kerberos realm name.</span></span> <span data-ttu-id="39aeb-131">С учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="39aeb-131">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39aeb-132">Связи</span><span class="sxs-lookup"><span data-stu-id="39aeb-132">Relationships</span></span>
<span data-ttu-id="39aeb-133">Нет</span><span class="sxs-lookup"><span data-stu-id="39aeb-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="39aeb-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="39aeb-134">JSON Representation</span></span>
<span data-ttu-id="39aeb-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39aeb-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosSingleSignOnSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosSingleSignOnSettings",
  "allowedAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "allowedUrls": [
    "String"
  ],
  "displayName": "String",
  "kerberosPrincipalName": "String",
  "kerberosRealm": "String"
}
```





