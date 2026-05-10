# Storyboard Prompt Generator

## 中文说明

Storyboard Prompt Generator 是一个 Codex skill。它可以把用户输入的一个创意想法，直接扩展成一组故事板类型的图像生成提示词。

这个 skill 适合生成广告故事板，导演分镜板，产品视觉规划表，角色设定板，场景设计板，社交媒体内容板，活动视觉提案板和品牌前期制作板。

## 主要能力

1. 根据一个想法生成多条可复制的完整提示词。

2. 默认输出 8 条故事板类型提示词。

3. 支持中文内容，适合生成带有中文标题和分区标签的视觉规划图。

4. 自动覆盖不同角度，例如商业广告，产品展示，动漫分镜，社媒内容，品牌提案，活动策划，角色设定和信息图。

5. 每条提示词都会强调 16:9 横版，清晰分区，故事板区域，色卡，材质样本，灯光情绪，镜头类型和避免真实品牌 Logo。

## 使用示例

```text
Use $storyboard-prompt-generator to turn “泰国冰汽水广告” into a set of storyboard style image prompts.
```

```text
使用 $storyboard-prompt-generator，把“未来城市智能雨伞广告”扩展成 8 条故事板视觉规划提示词。
```

```text
使用 $storyboard-prompt-generator，围绕“儿童科学实验课程”生成一组教育类视觉规划提示词。
```

## 输出内容

每次调用通常会得到：

1. 一组提示词标题。

2. 一个统一创意方向。

3. 多条可直接复制到图像生成工具中的完整提示词。

4. 每条提示词包含适用场景，例如广告故事板，产品规划板，动画分镜板，活动视觉板或品牌提案板。

## 安装方式

将本仓库放入 Codex skills 目录：

```powershell
git clone https://github.com/zhouwei713/storyboard-prompt-generator.git
Copy-Item .\storyboard-prompt-generator "$env:USERPROFILE\.codex\skills\" -Recurse
```

安装后，在 Codex 中使用 `$storyboard-prompt-generator` 调用。

## 文件结构

```text
storyboard-prompt-generator
  SKILL.md
  agents
    openai.yaml
  references
    prompt-patterns.md
```

## 设计原则

1. 用户只需要输入一个想法。

2. skill 直接输出提示词组。

3. 提示词要像真实广告导演或美术指导使用的前期制作板。

4. 画面要求专业，清晰，信息密度高，叙事连贯。

5. 生成图像时避免真实品牌 Logo，乱码文字，过度拥挤和无关人物抢镜。

## English

Storyboard Prompt Generator is a Codex skill that turns one creative idea into a set of storyboard style image generation prompts.

It is useful for advertising storyboards, director boards, product visual planning boards, character reference boards, scene design boards, social content boards, event proposal boards, and brand preproduction boards.

## Key Features

1. Generate multiple copy ready prompts from one idea.

2. Default to 8 storyboard style prompts.

3. Support Chinese visual board labels and concise in image text.

4. Cover varied creative directions, including commercial advertising, product planning, animation storyboard, social media content, brand proposal, event planning, character reference, and infographic style boards.

5. Keep each prompt focused on a 16:9 horizontal board, clear layout, storyboard panels, color palette, material samples, lighting notes, camera types, and logo safety.

## Example Usage

```text
Use $storyboard-prompt-generator to turn “Thai ice soda commercial” into a set of storyboard style image prompts.
```

```text
Use $storyboard-prompt-generator to generate visual planning prompts for “a futuristic smart umbrella campaign”.
```

```text
Use $storyboard-prompt-generator to create education themed storyboard prompts for “children's science experiment class”.
```

## Typical Output

Each run usually returns:

1. A prompt set title.

2. A concise creative direction.

3. Multiple complete prompts ready for image generation tools.

4. A use case label for each prompt, such as advertising storyboard, product planning board, animation storyboard, event visual board, or brand proposal board.

## Installation

Place this repository in your Codex skills directory:

```powershell
git clone https://github.com/zhouwei713/storyboard-prompt-generator.git
Copy-Item .\storyboard-prompt-generator "$env:USERPROFILE\.codex\skills\" -Recurse
```

Then invoke it in Codex with `$storyboard-prompt-generator`.

## Project Structure

```text
storyboard-prompt-generator
  SKILL.md
  agents
    openai.yaml
  references
    prompt-patterns.md
```

## Design Notes

1. The user should only need to provide one idea.

2. The skill should return a prompt set directly.

3. The prompts should feel like professional preproduction boards used by advertising directors or art directors.

4. The visual output should be polished, clear, information rich, and narratively coherent.

5. Prompts should avoid real brand logos, unreadable random text, overcrowded layouts, and irrelevant characters.
