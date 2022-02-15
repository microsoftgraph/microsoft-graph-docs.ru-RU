---
title: тип ресурса loginPageTextVisibilitySettings
description: Содержит сведения о брендинге организации.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f31973dad83f09305bdae6a9f9997b6af35d5049
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2022
ms.locfileid: "62805436"
---
# <a name="loginpagetextvisibilitysettings-resource-type"></a>тип ресурса loginPageTextVisibilitySettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Это сложный тип, который представляет различные тексты, которые можно скрыть на странице регистрации для клиента.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| hideCannotAccessYourAccount | Boolean | Параметр скрыть сброс пароля самообслуживаемой (SSPR) "Не может получить доступ к вашей учетной записи?" гиперссылка на входной форме. |
| hideForgotMyPassword | Boolean | Возможность скрыть гиперссылку сбросить пароль самообслуживки (SSPR) "Забыл пароль" в форме входного знака. |
| hideResetItNow | Boolean | Возможность скрыть гиперссылку самообслуживляемого сброса пароля (SSPR) в форме входной записи. |
| hideTermsOfUse | Boolean | Возможность скрыть гиперссылку "Условия использования" в подножке. |
| hidePrivacyAndCookies | Boolean | Возможность скрыть гиперссылку "Конфиденциальность & cookies" в подножке. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loginPageTextVisibilitySettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loginPageTextVisibilitySettings",
  "hideCannotAccessYourAccount": "Boolean",
  "hideForgotMyPassword": "Boolean",
  "hidePrivacyAndCookies": "Boolean",
  "hideResetItNow": "Boolean",
  "hideTermsOfUse": "Boolean"
}
```
