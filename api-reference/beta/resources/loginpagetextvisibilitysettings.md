---
title: Тип ресурса loginPageTextVisibilitySettings
description: Содержит сведения о фирменной символике организации.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9a18a8678db335b788ef170f97958de5154a1942
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441722"
---
# <a name="loginpagetextvisibilitysettings-resource-type"></a>Тип ресурса loginPageTextVisibilitySettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет различные текстовые строки, которые могут быть скрыты на странице входа для клиента.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| hideAccountResetCredentials | Boolean | Возможность скрыть гиперссылки самостоятельного сброса пароля (SSPR), такие как "Не удается получить доступ к учетной записи?", "Забыли пароль" и "Сбросить его сейчас" в форме входа. |
| hideCannotAccessYourAccount | Логическое | Возможность скрыть самостоятельный сброс пароля (SSPR) "Не удается получить доступ к учетной записи?" гиперссылка на форму входа. |
| hideForgotMyPassword | Логическое | Возможность скрыть гиперссылку самостоятельного сброса пароля (SSPR) "Забыли пароль" в форме входа. |
| hideResetItNow | Логическое | Возможность скрыть гиперссылку самостоятельного сброса пароля (SSPR) "сбросить сейчас" на форме входа. |
| hideTermsOfUse | Логическое | Возможность скрыть гиперссылку "Условия использования" в нижнем колонтитуле. |
| hidePrivacyAndCookies | Логическое | Возможность скрыть гиперссылку "Конфиденциальность & cookies" в нижнем колонтитуле. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loginPageTextVisibilitySettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loginPageTextVisibilitySettings",
  "hideAccountResetCredentials": "Boolean",
  "hideCannotAccessYourAccount": "Boolean",
  "hideForgotMyPassword": "Boolean",
  "hidePrivacyAndCookies": "Boolean",
  "hideResetItNow": "Boolean",
  "hideTermsOfUse": "Boolean"
}
```
